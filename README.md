# Extensiv (extensiv)

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

Extensiv (formerly 3PL Central, rebranded in 2022) is a cloud-native omnichannel fulfillment software company for third-party logistics providers (3PLs) and brands. Its platform combines warehouse management (3PL Warehouse Manager and Warehouse Manager), order management, inventory management, and integration tooling - built from the combination of 3PL Central, Skubana, Scout, and CartRover. The flagship developer surface is the 3PL Warehouse Manager REST API (auth server at `secure-wms.com/AuthServer`), which exposes orders, inventory, items, customers, receivers/ASN, stock summaries, and warehouses to external integrators. Access is provisioned with Client ID / Client Secret credentials that mint short-lived bearer tokens.

**Relationship note:** The SecureWMS / 3PL Warehouse Manager REST API itself is profiled in more detail in the sibling `all/3plcentral` entry. This entry documents the Extensiv company and platform and its relationship to that API rather than duplicating it. Resource endpoints here are honestly modeled from Extensiv's publicly documented resource areas; only the authentication endpoint is confirmed, because the full reference at `developer.extensiv.com` is a JavaScript-rendered developer portal that is effectively gated. Request REST API access via `api@extensiv.com`.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/extensiv/refs/heads/main/apis.yml)

## Tags

- 3PL
- Warehouse Management
- WMS
- Order Management
- Inventory Management
- Fulfillment
- Logistics
- Supply Chain

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### Extensiv Orders API

Create and retrieve sales/fulfillment orders in 3PL Warehouse Manager - the most common use of the API. Supports listing, filtering, creating, updating, and retrieving individual orders along with their order items and allocation state.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Orders
- Fulfillment
- Shipping

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Inventory API

Retrieve on-hand inventory and stock summaries, including inventory received on or before a given date and rolled-up availability by SKU. A primary read surface for keeping external systems in sync with warehouse stock.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Inventory
- Stock Summaries
- Availability

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Items API

Read the SKU/item master for a customer - the products a 3PL stores and ships. Items are scoped to a customer and carry identifiers, descriptions, and packaging attributes used across orders and inventory.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Items
- SKUs
- Catalog

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Customers API

List and retrieve the customers (the brands/merchants a 3PL serves) configured in a warehouse. Customers are the top-level tenant under which items, orders, and inventory are organized.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Customers
- Accounts
- Tenants

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Receivers (ASN) API

Manage inbound receivers / advance shipping notices (ASNs) - the expected inbound shipments a warehouse receives against. Create, list, and retrieve receivers and their line items to drive the receiving workflow.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Receivers
- ASN
- Receiving

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Warehouses API

List the physical warehouses/facilities configured on an account and their identifiers, used to scope inventory, orders, and receiving to a location.

- **Human URL:** [https://developer.extensiv.com/pages/3pl-wareshouse-manager.html](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- **Base URL:** `https://secure-wms.com`

#### Tags

- Warehouses
- Facilities
- Locations

#### Properties

- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [API Reference](https://developer.extensiv.com/pages/3pl-wareshouse-manager.html)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Extensiv Auth Token API

OAuth2-style token endpoint at `secure-wms.com/AuthServer`. A Base64 Client ID:Client Secret authorization header plus a grant_type mints a short-lived bearer access token (typically valid 30-60 minutes) that authorizes all other 3PL Warehouse Manager REST API calls. This endpoint is confirmed against Extensiv's public help documentation.

- **Human URL:** [https://help.extensiv.com/rest-api/getting-started-with-credential-management](https://help.extensiv.com/rest-api/getting-started-with-credential-management)
- **Base URL:** `https://secure-wms.com/AuthServer`

#### Tags

- Authentication
- OAuth2
- Tokens

#### Properties

- [Documentation](https://help.extensiv.com/rest-api/getting-started-with-credential-management)
- [API Reference](https://help.extensiv.com/rest-api/providing-rest-api-access)
- [OpenAPI](openapi/extensiv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/extensiv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/extensiv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/extensiv)
- [Website](https://www.extensiv.com)
- [Documentation](https://help.extensiv.com/en_US/rest-api)
- [Plans](plans/extensiv-plans-pricing.yml)
- [Rate Limits](rate-limits/extensiv-rate-limits.yml)
- [Fin Ops](finops/extensiv-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
