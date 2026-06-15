# Rapid7 (rapid7)

Rapid7 is a cybersecurity company providing the Insight Platform with products for vulnerability management (InsightVM), SIEM/XDR (InsightIDR), application security (InsightAppSec), cloud security (InsightCloudSec), and SOAR (InsightConnect). The Rapid7 Command/Insight Platform API exposes REST endpoints across regional hosts such as us.api.insight.rapid7.com for managing assets, vulnerabilities, investigations, and integrations. Authentication is performed with an organization or user API key passed in the `X-Api-Key` header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/rapid7/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/rapid7/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Security
- Vulnerability Management
- SIEM
- XDR
- Cloud Security
- SOAR
- Application Security

## Timestamps

- **Created:** 2026-05-11
- **Modified:** 2026-05-19

## APIs

### Rapid7 InsightVM Cloud API

REST API for the InsightVM vulnerability management product, exposing assets, scans, vulnerabilities, remediation projects, and reports. Authentication uses an Insight Platform API key in the `X-Api-Key` header; the regional base URL is selected per data residency.

- **Human URL:** [https://help.rapid7.com/insightvm/en-us/api/api.html](https://help.rapid7.com/insightvm/en-us/api/api.html)
- **Base URL:** `https://us.api.insight.rapid7.com/vm/v4`

#### Tags

- Vulnerability Management
- Assets
- Scans
- Remediation

#### Properties

- [Documentation](https://help.rapid7.com/insightvm/en-us/api/api.html)
- [Integrations  A P I](https://help.rapid7.com/insightvm/en-us/api/integrations.html)
- [Examples](https://github.com/rapid7/insightvm-api-examples)
- [Postman Collection](collections/insightappsec.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightappsec.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightidr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightidr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightvm-console-swagger.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightvm-console-swagger.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Rapid7 Insight Platform API

Cross-product REST API for the Insight Platform that covers user and key management, organizations, audit logs, and platform-level integrations. Authentication uses `X-Api-Key` against the regional endpoint (us, eu, ca, au, ap, jp).

- **Human URL:** [https://docs.rapid7.com/insight/api-overview/](https://docs.rapid7.com/insight/api-overview/)
- **Base URL:** `https://us.api.insight.rapid7.com`

#### Tags

- Identity
- Platform
- Organizations
- Audit

#### Properties

- [Documentation](https://docs.rapid7.com/insight/api-overview/)
- [Managing  A P I  Keys](https://docs.rapid7.com/insight/managing-platform-api-keys/)
- [Postman Collection](collections/insightappsec.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightappsec.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightidr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightidr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightvm-console-swagger.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightvm-console-swagger.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Rapid7 InsightIDR API

REST API for the InsightIDR SIEM/XDR product covering investigations, alerts, log search, threats, and SOC workflows. Authentication uses `X-Api-Key` against the regional Insight Platform endpoint.

- **Human URL:** [https://docs.rapid7.com/insightidr/api-overview/](https://docs.rapid7.com/insightidr/api-overview/)
- **Base URL:** `https://us.api.insight.rapid7.com/idr`

#### Tags

- SIEM
- XDR
- Investigations
- Alerts
- Logs

#### Properties

- [Documentation](https://docs.rapid7.com/insightidr/api-overview/)
- [Postman Collection](collections/insightappsec.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightappsec.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightidr.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightidr.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/insightvm-console-swagger.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/insightvm-console-swagger.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/rapid7)
- [Website](https://www.rapid7.com)
- [Documentation](https://docs.rapid7.com)
- [A P I  Overview](https://docs.rapid7.com/insight/api-overview/)
- [Pricing](https://www.rapid7.com/contact/)
- [Sign Up](https://insight.rapid7.com/)
- [GitHub Organization](https://github.com/rapid7)
- [Community](https://discuss.rapid7.com)
- [Support](https://www.rapid7.com/services/support/)
- [Status Page](https://status.rapid7.com)
- [M C P Server](https://github.com/rapid7/rapid7-bulk-export-mcp)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
