# Extensiv (extensiv)

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
