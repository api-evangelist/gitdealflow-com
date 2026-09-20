---
name: gitdealflow-lookup-startup-signal-rest
description: Look up a startup's engineering-acceleration signal over the free REST API (no MCP client needed), fall back to the bulk panel when the name is not tracked, and only then decide whether to spend a paid deep-signal credit.
api: openapi/gitdealflow-com-signals-openapi.yml
operations: [getSingleSignal, getSignals, getDiligenceDossier, getDeepSignal, getDeepSignalX402, getCredits]
method: generated
generated: '2026-09-19'
grounding: every operationId above exists verbatim in the provider's OpenAPI 3.1 (info.version 1.4.0); conventions from conventions/gitdealflow-com-conventions.yml, errors from errors/gitdealflow-com-problem-types.yml
---

# Look up a startup signal (REST)

Base URL `https://signals.gitdealflow.com`. Free routes need no credentials and are CORS-open;
the data is CC BY 4.0 — cite "VC Deal Flow Signal (signals.gitdealflow.com)" in anything you produce.

## Steps

1. **Single lookup** — `getSingleSignal`: `GET /api/signal?company=<display name or GitHub org slug>`.
   Matching is case-insensitive. Rate limit on this route is 30 requests/min/IP (429 + `Retry-After`).
   A tracked startup returns a `Startup` object (commitVelocity14d, commitVelocityChange,
   contributors, contributorGrowth, newRepos, signalType, githubUrl). A miss returns `found: false`
   — do not invent numbers; go to step 2.
2. **Not tracked? Search the panel** — `getSignals`: `GET /api/signals.json` (edge-cached one hour,
   ~190 KB). Scan `trending[]` and `sectors[].startups[]` for a near-match on `name` or `githubUrl`.
   If still absent, the company is outside the ~411-startup panel; say so and stop. Do NOT call the
   paid route hoping for a hit — misses are free there too, but the answer will be the same.
3. **Public diligence context (free)** — `getDiligenceDossier`: `GET /api/diligence.json?company=<name>`
   returns M&A history, public backers and the published signal, or 404 outside the corpus.
4. **Only if the user needs memo-grade output, spend a credit** — `getDeepSignal`:
   `POST /api/agent/deep-signal` with `{"name": "<name>"}` and `Authorization: Bearer gdf_v2.<customerId>.<hmac>`.
   Costs 1 credit (EUR 0.19) only when `found: true`; `401 missing_api_key` means no key was sent,
   `402` means the pack is empty (buy at https://signals.gitdealflow.com/agents/credits). Read the
   `X-Credits-Balance` response header and surface it to the user. Check the balance first with
   `getCredits` (`GET /api/account/credits`, same bearer) when the user asked you to stay under a budget.
   Wallet-holding agents with no human to top up credits use `getDeepSignalX402` instead:
   `POST /api/agent/deep-signal/x402`, expect `402` with an `accepts[]` block (USDC on Base,
   190000 atomic units = 0.19 USDC), sign EIP-3009 and retry with `X-PAYMENT`. 404 is never charged.

## Rules

- There is no reversal for a consumed credit; the only thing that prevents double-spend is the
  provider's `idempotentHint: true` on the tool and your own retry discipline — never retry a `200`.
- Errors are plain JSON `{ "error": "<code>", "message": "..." }`, not RFC 9457.
- Data refreshes weekly (Mondays); include the `period`/`citation` field from the response.
- This is a leading indicator, not investment advice, and private repositories are invisible to it.
