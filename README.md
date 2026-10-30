# Extensiv

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

Extensiv (formerly 3PL Central, rebranded in 2022) is a cloud-native omnichannel fulfillment software company for third-party logistics providers (3PLs) and brands. Its platform combines warehouse management (3PL Warehouse Manager and Warehouse Manager), order management, inventory management, and integration tooling - built from the combination of 3PL Central, Skubana, Scout, and CartRover. The flagship developer surface is the 3PL Warehouse Manager REST API (auth server at secure-wms.com/AuthServer), which exposes orders, inventory, items, customers, receivers/ASN, stock summaries, and warehouses to external integrators. Access is provisioned with Client ID / Client Secret credentials that mint short-lived bearer tokens. NOTE - the SecureWMS/3PL Warehouse Manager REST API itself is documented in more detail in the sibling all/3plcentral entry; this entry profiles the Extensiv company and platform and its relationship to that API.

**Areas:** 3PL · Warehouse Management · WMS · Order Management · Inventory · Fulfillment · Logistics · Supply Chain · Order · SecureWMS · Extensiv

## Extensiv on APIs.io

Everything profiled for Extensiv is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/extensiv/](https://apis.io/providers/extensiv/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Extensiv Authentication API](https://apis.io/apis/extensiv/extensiv-authentication-api/) — OAuth2-style token endpoint (endpointsConfirmed).
- [Extensiv Customers API](https://apis.io/apis/extensiv/extensiv-customers-api/) — Customer/tenant accounts (endpointsModeled).
- [Extensiv Inventory API](https://apis.io/apis/extensiv/extensiv-inventory-api/) — On-hand inventory and stock summaries (endpointsModeled).
- [Extensiv Items API](https://apis.io/apis/extensiv/extensiv-items-api/) — Customer SKU/item master (endpointsModeled).
- [Extensiv Orders API](https://apis.io/apis/extensiv/extensiv-orders-api/) — Sales/fulfillment orders (endpointsModeled).
- [Extensiv Receivers API](https://apis.io/apis/extensiv/extensiv-receivers-api/) — Inbound receivers / ASNs (endpointsModeled).
- [Extensiv Warehouses API](https://apis.io/apis/extensiv/extensiv-warehouses-api/) — Physical facilities (endpointsModeled).

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Extensiv Agentic Access](https://apis.io/agentic-access/extensiv/extensiv-agentic-access/)

#### Collections (8)

Postman and Open Collection request collections.

- [Extensiv 3PL Warehouse Manager API (modeled)](https://apis.io/collections/extensiv/open-extensiv/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication API](https://apis.io/collections/extensiv/open-extensiv-authentication-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Customers API](https://apis.io/collections/extensiv/open-extensiv-customers-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Inventory API](https://apis.io/collections/extensiv/open-extensiv-inventory-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Items API](https://apis.io/collections/extensiv/open-extensiv-items-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Orders API](https://apis.io/collections/extensiv/open-extensiv-orders-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Receivers API](https://apis.io/collections/extensiv/open-extensiv-receivers-api/)
- [Extensiv 3PL Warehouse Manager API (modeled) Authentication Warehouses API](https://apis.io/collections/extensiv/open-extensiv-warehouses-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Extensiv Authentication](https://apis.io/security/extensiv/extensiv-authentication/)
- [Extensiv Domain Security](https://apis.io/security/extensiv/extensiv-domain-security/)
- [Extensiv Trust Center](https://apis.io/security/extensiv/extensiv-trust-center/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Extensiv Plans Pricing](https://apis.io/plans/extensiv/extensiv-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Extensiv Rate Limits](https://apis.io/rate-limits/extensiv/extensiv-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Extensiv Finops](https://apis.io/finops/extensiv/extensiv-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.extensiv.com)
- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [Blog](https://www.extensiv.com/blog)
- [GitHub](https://github.com/tpl-central)

## API Evangelist rating

**Kin Score 28.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 45.8 |
| Contract governance | 0.0 |
| Operational transparency | 13.2 |
| Developer ergonomics | 31.0 |
| Access clarity | 15.8 |

**Agent readiness 20.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/extensiv/](https://apis.io/providers/extensiv/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Extensiv: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/extensiv/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
