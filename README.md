# Rapid7

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

**Areas:** Security · Vulnerability Management · SIEM · XDR · Cloud Security · SOAR · Application Security

## Rapid7 on APIs.io

Everything profiled for Rapid7 is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/rapid7/](https://apis.io/providers/rapid7/)** — or go straight to one of the APIs or properties below.

### APIs (50)

- [Rapid7 InsightVM Cloud API](https://apis.io/apis/rapid7/insightvm-api/) — REST API for the InsightVM vulnerability management product, exposing assets, scans, vulnerabilities, remediation projects, and reports. Authentication uses…
- [Rapid7 Insight Platform API](https://apis.io/apis/rapid7/insight-platform-api/) — Cross-product REST API for the Insight Platform that covers user and key management, organizations, audit logs, and platform-level integrations.…
- [Rapid7 InsightIDR API](https://apis.io/apis/rapid7/insightidr-api/) — REST API for the InsightIDR SIEM/XDR product covering investigations, alerts, log search, threats, and SOC workflows. Authentication uses `X-Api-Key`…
- [Rapid7 Accounts API](https://apis.io/apis/rapid7/rapid7-accounts-api/) — An API used to find and search InsightIDR accounts. See https://docs.rapid7.com/insightidr/users-and-accounts-on-your-domain for further information on…
- [Rapid7 Administration API](https://apis.io/apis/rapid7/rapid7-administration-api/) — Provides access administrative operations and procedures.
- [Rapid7 Apps API](https://apis.io/apis/rapid7/rapid7-apps-api/) — An App <i>owns</i> Scan Configs, Schedules, Scans and Vulnerabilities; you must create an App in order to create any of these other resources. Consequently,…
- [Rapid7 Asset API](https://apis.io/apis/rapid7/rapid7-asset-api/) — Resources and operations for managing assets. Assets can be created under the <a href="#operation/createAssetUsingPOST">Site Assets</a> resource.
- [Rapid7 Asset Discovery API](https://apis.io/apis/rapid7/rapid7-asset-discovery-api/) — Resources for managing and viewing the mechanisms used to automatically discover assets.
- [Rapid7 Asset Group API](https://apis.io/apis/rapid7/rapid7-asset-group-api/) — Resources and operations for managing asset groups.
- [Rapid7 Assets API](https://apis.io/apis/rapid7/rapid7-assets-api/) — An API used to find and search InsightIDR assets. See https://docs.rapid7.com/insightidr/assets-on-your-domain for further information on assets.
- [Rapid7 Attachments API](https://apis.io/apis/rapid7/rapid7-attachments-api/) — An API used to upload, list, download and delete attachments. For example, the create API can be used to upload an attachment.
- [Rapid7 Attack Templates API](https://apis.io/apis/rapid7/rapid7-attack-templates-api/) — An Attack Template describes <i>if</i> and <i>how</i> Attacks should be executed during the execution of a Scan. There exist pre-defined, system-provided…
- [Rapid7 Blackouts API](https://apis.io/apis/rapid7/rapid7-blackouts-api/) — A blackout is a period of time when all scanning activities for the specified scope are blocked. A blackout can be scoped globally or to a specific App,…
- [Rapid7 Collectors API](https://apis.io/apis/rapid7/rapid7-collectors-api/) — An API used to manage collectors for an organization.
- [Rapid7 Comments API](https://apis.io/apis/rapid7/rapid7-comments-api/) — An API used to find, create, and delete comments. For example, these APIs can be used to create a comment for a particular investigation.
- [Rapid7 Community Threats API](https://apis.io/apis/rapid7/rapid7-community-threats-api/) — An API used to add and replace indicators for Community Threats. See https://insightidr.help.rapid7.com/docs/threats#section-threat-api for further…
- [Rapid7 Credential API](https://apis.io/apis/rapid7/rapid7-credential-api/) — Resources and operations for managing shared credentials.
- [Rapid7 Engine Groups API](https://apis.io/apis/rapid7/rapid7-engine-groups-api/) — An Engine Group is a resource which defines a container for a logical grouping of Engines and therefore the purpose of assigning Scans to one of those…
- [Rapid7 Engines API](https://apis.io/apis/rapid7/rapid7-engines-api/) — An Engine encapsulates the state and high-level attributes of the components which may be installed and running on a specific On-Premise host. The status of…
- [Rapid7 Files API](https://apis.io/apis/rapid7/rapid7-files-api/) — Files are used primarily to manage content that can be required to successfully scan an App. For example, many supported methods of configuring…
- [Rapid7 Health Metrics API](https://apis.io/apis/rapid7/rapid7-health-metrics-api/) — An API used to retrieve health metrics of an organization.
- [Rapid7 Investigations API](https://apis.io/apis/rapid7/rapid7-investigations-api/) — The Investigations API from Rapid7 — 4 operation(s) for investigations.
- [Rapid7 Local Accounts API](https://apis.io/apis/rapid7/rapid7-local-accounts-api/) — An API used to find and search InsightIDR local accounts. See https://docs.rapid7.com/insightidr/users-and-accounts-on-your-domain for further information…
- [Rapid7 Policy API](https://apis.io/apis/rapid7/rapid7-policy-api/) — Resources and operations for managing policies.
- [Rapid7 Policy Override API](https://apis.io/apis/rapid7/rapid7-policy-override-api/) — Policy Override Resource Controller
- [Rapid7 Remediation API](https://apis.io/apis/rapid7/rapid7-remediation-api/) — Resources for determining the details required to remediate vulnerabilities.
- [Rapid7 Report API](https://apis.io/apis/rapid7/rapid7-report-api/) — Resources and operations for managing and generating reports. Reports are broadly categorized into `document`, `export`, and `file` types. `document`…
- [Rapid7 Reports API](https://apis.io/apis/rapid7/rapid7-reports-api/) — Reports provide the ability to share information with stakeholders at both scan and app levels. The following table lists the report templates and the…
- [Rapid7 Root API](https://apis.io/apis/rapid7/rapid7-root-api/) — Provides access to primary entry point for discovering the available resources in this API.
- [Rapid7 Scan API](https://apis.io/apis/rapid7/rapid7-scan-api/) — Resources and operations for managing scans.
- [Rapid7 Scan Configs API](https://apis.io/apis/rapid7/rapid7-scan-configs-api/) — A Scan Config defines all the necessary information required to perform a Scan of an App. An App <i>must</i> be created prior to creating a Scan Config. It…
- [Rapid7 Scan Engine API](https://apis.io/apis/rapid7/rapid7-scan-engine-api/) — Resources and operations for managing scan engines.
- [Rapid7 Scan Template API](https://apis.io/apis/rapid7/rapid7-scan-template-api/) — Scan Template Resource Controller
- [Rapid7 Scans API](https://apis.io/apis/rapid7/rapid7-scans-api/) — A Scan encapsulates all the information for a single execution of the criteria defined in the provided Scan Config. An App and a Scan Config <i>must</i> be…
- [Rapid7 Schedules API](https://apis.io/apis/rapid7/rapid7-schedules-api/) — A Schedule defines the automated execution of a Scan, using a specified Scan Config. Both the App and Scan Config must be created prior to creating a…
- [Rapid7 Search API](https://apis.io/apis/rapid7/rapid7-search-api/) — A global Search API is exposed to facilitate the execution of user-defined queries that can perform a Search across the supported resource types exposed via…
- [Rapid7 Site API](https://apis.io/apis/rapid7/rapid7-site-api/) — Resources and operations for managing sites.
- [Rapid7 Tag API](https://apis.io/apis/rapid7/rapid7-tag-api/) — Resources and operations for managing tags.
- [Rapid7 Tags API](https://apis.io/apis/rapid7/rapid7-tags-api/) — Tags are customer-defined labels that can be used for a variety of purposes. The management of Tags is performed by this API, and other APIs facilitate…
- [Rapid7 Targets API](https://apis.io/apis/rapid7/rapid7-targets-api/) — A Target essentially specifies an allowlisted Fully Qualified Domain Name (FQDN) which can be Scanned by InsightAppSec. A Target can be created, edited and…
- [Rapid7 User API](https://apis.io/apis/rapid7/rapid7-user-api/) — Resources and operations for managing users, permissions, and privileges.
- [Rapid7 Users API](https://apis.io/apis/rapid7/rapid7-users-api/) — An API used to find and search InsightIDR users. See https://docs.rapid7.com/insightidr/users-and-accounts-on-your-domain for further information on users.
- [Rapid7 Variances Documentation API](https://apis.io/apis/rapid7/rapid7-variances-documentation-api/) — The Variances Documentation API from Rapid7 — 2 operation(s) for variances documentation.
- [Rapid7 Vulnerabilities API](https://apis.io/apis/rapid7/rapid7-vulnerabilities-api/) — A Vulnerability is a resource that encapsulates any information found by any Scan over the lifetime of an App, that <i>may</i> identify where and how an App…
- [Rapid7 Vulnerability API](https://apis.io/apis/rapid7/rapid7-vulnerability-api/) — Resources and operations for viewing vulnerability content and managing exceptions.
- [Rapid7 Vulnerability Check API](https://apis.io/apis/rapid7/rapid7-vulnerability-check-api/) — Resources and operations for view vulnerability checks that can be run as a part of vulnerability content.
- [Rapid7 Vulnerability Comments API](https://apis.io/apis/rapid7/rapid7-vulnerability-comments-api/) — A Vulnerability Comment is a resource that allows users to add context to the Vulnerability.
- [Rapid7 Vulnerability Exception API](https://apis.io/apis/rapid7/rapid7-vulnerability-exception-api/) — Vulnerability Exception Resource Controller
- [Rapid7 Vulnerability History API](https://apis.io/apis/rapid7/rapid7-vulnerability-history-api/) — A Vulnerability History resource represents the change applied to a specific Vulnerability at a point of time in its existence.
- [Rapid7 Vulnerability Result API](https://apis.io/apis/rapid7/rapid7-vulnerability-result-api/) — Resources and operations for retrieving vulnerability results on assessed assets.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/rapid7/](https://apis.io/graphqls/rapid7/rapid7-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [MCP Server](https://apis.io/servers/rapid7/mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Rapid7 Agentic Access](https://apis.io/agentic-access/rapid7/rapid7-agentic-access/)

#### JSON Schema (205)

The data models the API reads and writes.

- [AccountV2](https://apis.io/schemas/rapid7/rapid7-accountv2/)
- [AddCollectorRequest](https://apis.io/schemas/rapid7/rapid7-addcollectorrequest/)
- [AddCollectorResponse](https://apis.io/schemas/rapid7/rapid7-addcollectorresponse/)
- [AlertInfo](https://apis.io/schemas/rapid7/rapid7-alertinfo/)
- [AlfDataFile](https://apis.io/schemas/rapid7/rapid7-alfdatafile/)
- [app](https://apis.io/schemas/rapid7/rapid7-app/)
- [AssetV2](https://apis.io/schemas/rapid7/rapid7-assetv2/)
- [Assignee](https://apis.io/schemas/rapid7/rapid7-assignee/)
- [AssignUserToInvestigationRequest](https://apis.io/schemas/rapid7/rapid7-assignusertoinvestigationrequest/)
- [Attachment](https://apis.io/schemas/rapid7/rapid7-attachment/)
- [attack_template](https://apis.io/schemas/rapid7/rapid7-attack-template/)
- [AttackDocumentation](https://apis.io/schemas/rapid7/rapid7-attackdocumentation/)
- [AttackerConfig](https://apis.io/schemas/rapid7/rapid7-attackerconfig/)
- [AttackMetadata](https://apis.io/schemas/rapid7/rapid7-attackmetadata/)
- [AttackModule](https://apis.io/schemas/rapid7/rapid7-attackmodule/)
- [AttackTemplate](https://apis.io/schemas/rapid7/rapid7-attacktemplate/)
- [AuthConfig](https://apis.io/schemas/rapid7/rapid7-authconfig/)
- [AutoSequenceConfig](https://apis.io/schemas/rapid7/rapid7-autosequenceconfig/)
- [BinaryContentType](https://apis.io/schemas/rapid7/rapid7-binarycontenttype/)
- [BinaryExtension](https://apis.io/schemas/rapid7/rapid7-binaryextension/)
- [Blackout](https://apis.io/schemas/rapid7/rapid7-blackout/)
- [BrowserDoNotDownloadContentType](https://apis.io/schemas/rapid7/rapid7-browserdonotdownloadcontenttype/)
- [BrowserDoNotDownloadExtension](https://apis.io/schemas/rapid7/rapid7-browserdonotdownloadextension/)
- [BrowserDownloadAllowlist](https://apis.io/schemas/rapid7/rapid7-browserdownloadallowlist/)
- [BrowserFormLoginConfig](https://apis.io/schemas/rapid7/rapid7-browserformloginconfig/)
- …and 180 more published on APIs.io

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Rapid7 Structure](https://apis.io/json-structure/rapid7/rapid7-structure/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Rapid7 Domain Vocabulary](https://apis.io/vocabularies/rapid7/rapid7-vocabulary/)

#### Examples (4)

Example requests and responses.

- [Rapid7 Addindicators Example](https://apis.io/examples/rapid7/rapid7-addindicators-example/)
- [Rapid7 Createcommunitythreat Example](https://apis.io/examples/rapid7/rapid7-createcommunitythreat-example/)
- [Rapid7 Getmetrics Example](https://apis.io/examples/rapid7/rapid7-getmetrics-example/)
- [Rapid7 Replaceindicators Example](https://apis.io/examples/rapid7/rapid7-replaceindicators-example/)

#### Collections (50)

Postman and Open Collection request collections.

- [InsightAppSec API](https://apis.io/collections/rapid7/open-insightappsec/)
- [InsightIDR API](https://apis.io/collections/rapid7/open-insightidr/)
- [InsightVM API](https://apis.io/collections/rapid7/open-insightvm-console-swagger/)
- [InsightAppSec Accounts API](https://apis.io/collections/rapid7/open-rapid7-accounts-api/)
- [InsightAppSec Accounts Administration API](https://apis.io/collections/rapid7/open-rapid7-administration-api/)
- [InsightAppSec Accounts Apps API](https://apis.io/collections/rapid7/open-rapid7-apps-api/)
- [InsightAppSec Accounts Asset API](https://apis.io/collections/rapid7/open-rapid7-asset-api/)
- [InsightAppSec Accounts Asset Discovery API](https://apis.io/collections/rapid7/open-rapid7-asset-discovery-api/)
- [InsightAppSec Accounts Asset Group API](https://apis.io/collections/rapid7/open-rapid7-asset-group-api/)
- [InsightAppSec Accounts Assets API](https://apis.io/collections/rapid7/open-rapid7-assets-api/)
- [InsightAppSec Accounts Attachments API](https://apis.io/collections/rapid7/open-rapid7-attachments-api/)
- [InsightAppSec Accounts Attack Templates API](https://apis.io/collections/rapid7/open-rapid7-attack-templates-api/)
- [InsightAppSec Accounts Blackouts API](https://apis.io/collections/rapid7/open-rapid7-blackouts-api/)
- [InsightAppSec Accounts Collectors API](https://apis.io/collections/rapid7/open-rapid7-collectors-api/)
- [InsightAppSec Accounts Comments API](https://apis.io/collections/rapid7/open-rapid7-comments-api/)
- [InsightAppSec Accounts Community Threats API](https://apis.io/collections/rapid7/open-rapid7-community-threats-api/)
- [InsightAppSec Accounts Credential API](https://apis.io/collections/rapid7/open-rapid7-credential-api/)
- [InsightAppSec Accounts Engine Groups API](https://apis.io/collections/rapid7/open-rapid7-engine-groups-api/)
- [InsightAppSec Accounts Engines API](https://apis.io/collections/rapid7/open-rapid7-engines-api/)
- [InsightAppSec Accounts Files API](https://apis.io/collections/rapid7/open-rapid7-files-api/)
- [InsightAppSec Accounts Health Metrics API](https://apis.io/collections/rapid7/open-rapid7-health-metrics-api/)
- [InsightAppSec Accounts Investigations API](https://apis.io/collections/rapid7/open-rapid7-investigations-api/)
- [InsightAppSec Accounts Local Accounts API](https://apis.io/collections/rapid7/open-rapid7-local-accounts-api/)
- [InsightAppSec Accounts Policy API](https://apis.io/collections/rapid7/open-rapid7-policy-api/)
- [InsightAppSec Accounts Policy Override API](https://apis.io/collections/rapid7/open-rapid7-policy-override-api/)
- …and 25 more published on APIs.io

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Rapid7 — jsonschema rules](https://apis.io/rules/rapid7/rapid7-jsonschema-spectral-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Rapid7 Authentication](https://apis.io/security/rapid7/rapid7-authentication/)
- [Rapid7 Domain Security](https://apis.io/security/rapid7/rapid7-domain-security/)
- [Rapid7 Vulnerability Disclosure](https://apis.io/security/rapid7/rapid7-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Rapid7 Plans Pricing](https://apis.io/plans/rapid7/rapid7-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Rapid7 Rate Limits](https://apis.io/rate-limits/rapid7/rapid7-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Rapid7 Finops](https://apis.io/finops/rapid7/rapid7-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.rapid7.com)
- [Documentation](https://docs.rapid7.com)
- [Pricing](https://www.rapid7.com/contact/)
- [Support](https://www.rapid7.com/services/support/)
- [Blog](https://www.rapid7.com/rss.xml)
- [GitHub](https://github.com/rapid7)
- [Status](https://status.rapid7.com)

## API Evangelist rating

**Kin Score 35.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 70.0 |
| Contract quality | 54.3 |
| Contract governance | 9.8 |
| Operational transparency | 23.7 |
| Developer ergonomics | 26.2 |
| Access clarity | 28.9 |

**Agent readiness 29.3** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
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

**Regulatory alignment 17.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/rapid7/](https://apis.io/providers/rapid7/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Rapid7: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/rapid7/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
