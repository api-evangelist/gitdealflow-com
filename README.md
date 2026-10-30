# GitDealFlow

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

GitDealFlow (also published as VC Deal Flow Signal) is a deal-flow signal tool for angel, scout and seed investors that reads public GitHub engineering activity across 400+ venture-backed startup organizations in 15 sectors and ranks the ones accelerating, historically 3-6 weeks before a fundraise announcement. The data is published free under CC BY 4.0 through a no-auth REST API described by an OpenAPI 3.1 document, a hosted MCP server (Streamable HTTP plus an npm stdio package), an A2A JSON-RPC agent with a published agent card, an NLWeb endpoint, JSON/CSV/ NDJSON bulk exports and an RSS feed, with one paid deep-signal endpoint metered by credit-pack key or x402 USDC micropayments. Operated pseudonymously from Cyprus by "The Data Nerd"; methodology published on SSRN.

**Areas:** Venture Capital · Deal Flow · Startups · GitHub · Alternative Data · Investing · MCP · Agents · Developer Tools · A2A

## GitDealFlow on APIs.io

Everything profiled for GitDealFlow is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/gitdealflow-com/](https://apis.io/providers/gitdealflow-com/)** — or go straight to one of the APIs or properties below.

### APIs (18)

- [VC Deal Flow Signal MCP Server](https://apis.io/apis/gitdealflow-com/vc-deal-flow-signal-mcp-server/) — Hosted Model Context Protocol server (protocol 2025-06-18, Streamable HTTP) exposing 12 read-only tools, 3 resources and 7 prompts over the same signal…
- [GitDealFlow A2A Agent](https://apis.io/apis/gitdealflow-com/gitdealflow-a2a-agent/) — Agent-to-Agent (A2A 0.3.0) JSON-RPC 2.0 endpoint implementing message/send, tasks/get and tasks/cancel over the signal panel, executing synchronously;…
- [GitDealFlow NLWeb Endpoint](https://apis.io/apis/gitdealflow-com/gitdealflow-nlweb-endpoint/) — Microsoft NLWeb-compatible conversational endpoint: POST a natural-language query and receive schema.org-typed JSON-LD (ItemList, Organization, Article,…
- [GitDealFlow Agents API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-agents-api/) — Agent / MCP discovery surfaces
- [GitDealFlow Answer API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-answer-api/) — Citation-ready Q&A retrieval
- [GitDealFlow Badges API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-badges-api/) — SVG badges for embeds
- [GitDealFlow Brand API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-brand-api/) — The brand API from GitDealFlow — 1 operation(s) for brand.
- [GitDealFlow Business Model API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-business-model-api/) — The business-model API from GitDealFlow — 1 operation(s) for business-model.
- [GitDealFlow Citation API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-citation-api/) — Reference-manager exports
- [GitDealFlow Community API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-community-api/) — The community API from GitDealFlow — 1 operation(s) for community.
- [GitDealFlow Deep Signal API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-deep-signal-api/) — Paid per-request enriched signals
- [GitDealFlow Glossary API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-glossary-api/) — Controlled-vocabulary term definitions
- [GitDealFlow Markets API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-markets-api/) — Open prediction markets
- [GitDealFlow Meta API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-meta-api/) — Pricing, changelog, dataset
- [GitDealFlow Methodology API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-methodology-api/) — Reproducible signal-computation methodology
- [GitDealFlow Scout API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-scout-api/) — Scout score receipts and prediction
- [GitDealFlow Search API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-search-api/) — On-site search across all content
- [GitDealFlow Signals API](https://apis.io/apis/gitdealflow-com/gitdealflow-com-signals-api/) — Startup engineering acceleration data

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [VC Deal Flow Signal](https://apis.io/servers/gitdealflow-com/vc-deal-flow-signal/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Gitdealflow Com Agentic Access](https://apis.io/agentic-access/gitdealflow-com/gitdealflow-com-agentic-access/)

#### Overlays (16)

OpenAPI overlays, including conversational phrasing for each operation.

- [Gitdealflow Com Agents Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-agents-api-phrasing-overlay/)
- [Gitdealflow Com Answer Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-answer-api-phrasing-overlay/)
- [Gitdealflow Com Badges Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-badges-api-phrasing-overlay/)
- [Gitdealflow Com Brand Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-brand-api-phrasing-overlay/)
- [Gitdealflow Com Business Model Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-business-model-api-phrasing-overlay/)
- [Gitdealflow Com Citation Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-citation-api-phrasing-overlay/)
- [Gitdealflow Com Community Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-community-api-phrasing-overlay/)
- [Gitdealflow Com Deep Signal Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-deep-signal-api-phrasing-overlay/)
- [Gitdealflow Com Glossary Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-glossary-api-phrasing-overlay/)
- [Gitdealflow Com Markets Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-markets-api-phrasing-overlay/)
- [Gitdealflow Com Meta Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-meta-api-phrasing-overlay/)
- [Gitdealflow Com Methodology Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-methodology-api-phrasing-overlay/)
- [Gitdealflow Com Scout Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-scout-api-phrasing-overlay/)
- [Gitdealflow Com Search Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-search-api-phrasing-overlay/)
- [Gitdealflow Com Signals Api Phrasing Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-signals-api-phrasing-overlay/)
- [Gitdealflow Com Signals Overlay](https://apis.io/overlays/gitdealflow-com/gitdealflow-com-signals-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Gitdealflow Com Authentication](https://apis.io/security/gitdealflow-com/gitdealflow-com-authentication/)
- [Gitdealflow Com Domain Security](https://apis.io/security/gitdealflow-com/gitdealflow-com-domain-security/)
- [Gitdealflow Com Vulnerability Disclosure](https://apis.io/security/gitdealflow-com/gitdealflow-com-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Gitdealflow Com Scopes](https://apis.io/scopes/gitdealflow-com/gitdealflow-com-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Gitdealflow Com Plans Pricing](https://apis.io/plans/gitdealflow-com/gitdealflow-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Gitdealflow Com Rate Limits](https://apis.io/rate-limits/gitdealflow-com/gitdealflow-com-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://gitdealflow.com/)
- [Documentation](https://signals.gitdealflow.com/developers)
- [Getting started](https://signals.gitdealflow.com/agents.md)
- [API reference](https://signals.gitdealflow.com/api/openapi.json)
- [Pricing](https://signals.gitdealflow.com/pricing)
- [Support](https://signals.gitdealflow.com/support)
- [Blog](https://signals.gitdealflow.com/blog)
- [Terms of service](https://gitdealflow.com/terms)
- [Privacy policy](https://gitdealflow.com/privacy)
- [GitHub](https://github.com/kindrat86)
- [Status](https://signals.gitdealflow.com/uptime)

## API Evangelist rating

**Kin Score 68.2** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 47.0 |
| Contract governance | 18.2 |
| Operational transparency | 78.9 |
| Developer ergonomics | 76.2 |
| Access clarity | 76.3 |

**Agent readiness 45.8** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | conformant |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 59.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/gitdealflow-com/](https://apis.io/providers/gitdealflow-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for GitDealFlow: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/gitdealflow-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
