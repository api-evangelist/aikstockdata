# 한국주식데이터 (aikstockdata)

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

An automated Korean equities open-data publisher. Each trading day it compiles DART filings and T+1 (previous-session) closing prices for KOSPI/KOSDAQ/KONEX names and re-publishes them as machine-readable JSON/CSV files, refreshed once per trading day at 18:10 KST. Free, keyless, and unauthenticated, with a REST/static-file API (OpenAPI 3.1), a hosted MCP server, and an llms.txt.

**Areas:** South Korea · Stock Market · Financial Data · Open Data · Dart · kospi · kosdaq · konex · Filings · Stocks · MCP · llms-txt

## 한국주식데이터 (aikstockdata) on APIs.io

Everything profiled for 한국주식데이터 (aikstockdata) is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/aikstockdata/](https://apis.io/providers/aikstockdata/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [한국주식데이터 (aikstockdata) Data API](https://apis.io/apis/aikstockdata/aikstockdata-data-api/) — The Data API from 한국주식데이터 (aikstockdata) — 37 operation(s) for data.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [mcp](https://apis.io/servers/aikstockdata/mcp/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Aikstockdata Agentic Access](https://apis.io/agentic-access/aikstockdata/aikstockdata-agentic-access/)

#### JSON Schema (9)

The data models the API reads and writes.

- [post-filing price paths (/data/public/disclosure_impact.json)](https://apis.io/schemas/aikstockdata/aikstockdata-disclosure_impact.schema/)
- [disclosure briefing (/data/public/disclosures.json)](https://apis.io/schemas/aikstockdata/aikstockdata-disclosures.schema/)
- [earnings ledger (/data/public/earnings.json)](https://apis.io/schemas/aikstockdata/aikstockdata-earnings.schema/)
- [excluded stocks (/data/public/excluded.json)](https://apis.io/schemas/aikstockdata/aikstockdata-excluded.schema/)
- [slim quotes (/data/public/quotes_slim.json)](https://apis.io/schemas/aikstockdata/aikstockdata-quotes_slim.schema/)
- [rankings (/data/public/rankings.json)](https://apis.io/schemas/aikstockdata/aikstockdata-rankings.schema/)
- [screening rows (/data/public/screen.json)](https://apis.io/schemas/aikstockdata/aikstockdata-screen.schema/)
- [per-stock JSON (/data/public/s/{code}.json)](https://apis.io/schemas/aikstockdata/aikstockdata-stock.schema/)
- [daily digest (/data/public/today.json)](https://apis.io/schemas/aikstockdata/aikstockdata-today.schema/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Aikstockdata Openapi Overlay](https://apis.io/overlays/aikstockdata/aikstockdata-openapi-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Moved to /providers/aikstockdata/](https://apis.io/rules/aikstockdata/aikstockdata-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Aikstockdata Authentication](https://apis.io/security/aikstockdata/aikstockdata-authentication/)
- [Aikstockdata Domain Security](https://apis.io/security/aikstockdata/aikstockdata-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Aikstockdata Plans Pricing](https://apis.io/plans/aikstockdata/aikstockdata-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Aikstockdata Rate Limits](https://apis.io/rate-limits/aikstockdata/aikstockdata-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://aikstockdata.com/)
- [Documentation](https://aikstockdata.com/ai)
- [Support](https://aikstockdata.com/about)
- [Changelog](https://aikstockdata.com/notices)
- [Blog](https://aikstockdata.com/feed.xml)
- [Terms of service](https://aikstockdata.com/terms)
- [Privacy policy](https://aikstockdata.com/privacy)
- [Status](https://aikstockdata.com/status)

## API Evangelist rating

**Kin Score 48.4** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 50.8 |
| Contract governance | 18.2 |
| Operational transparency | 34.2 |
| Developer ergonomics | 58.9 |
| Access clarity | 42.1 |

**Agent readiness 37.2** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | verified |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | — |

**Regulatory alignment 24.5** — Government & Public Sector

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/aikstockdata/](https://apis.io/providers/aikstockdata/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for 한국주식데이터 (aikstockdata): the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/aikstockdata/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
