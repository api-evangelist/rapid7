# Rapid7 (rapid7)

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
