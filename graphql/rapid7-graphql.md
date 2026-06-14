# Rapid7 GraphQL Schema

This conceptual GraphQL schema represents the Rapid7 Insight Platform API surface, covering InsightVM (vulnerability management), InsightIDR (SIEM/XDR), and InsightConnect (SOAR). The schema is derived from the Rapid7 REST API documentation at https://docs.rapid7.com/insight/api-documentation/ and models the core entities, relationships, and operations across the Rapid7 product suite.

## Provider

- **Name:** Rapid7
- **Products:** InsightVM, InsightIDR, InsightConnect, InsightAppSec, InsightCloudSec
- **Base URL:** https://us.api.insight.rapid7.com
- **Authentication:** API Key via `X-Api-Key` header
- **Documentation:** https://docs.rapid7.com/insight/api-overview/

## Schema Coverage

The schema covers 65+ named types organized into the following domains:

### Asset Management
Types: `Asset`, `AssetSummary`, `AssetTag`, `AssetGroup`, `IPAddress`, `HostName`, `OperatingSystem`, `Service`, `Port`, `Software`, `SoftwareVersion`

### Vulnerability Management
Types: `Vulnerability`, `VulnDetails`, `CVE`, `CVSS`, `ExploitAvailability`, `Severity`, `Risk`, `RiskScore`, `Assessment`, `AssessmentSummary`

### Scanning
Types: `Scan`, `ScanDetails`, `ScanEngine`, `ScanStatus`, `ScanPolicy`, `Site`, `SiteDetails`, `SiteAssets`, `Discovery`, `Connection`

### Credentials
Types: `Credential`, `CredentialDetails`, `SharedCredential`, `SiteCredential`

### Exploit Intelligence
Types: `Exploit`, `ExploitDetails`, `ExploitModule`, `MetasploitModule`

### Reporting
Types: `Report`, `ReportTemplate`, `ReportSchedule`, `ReportConfig`

### Policy & Compliance
Types: `Policy`, `PolicyControl`, `PolicyOverride`, `PolicyCheck`

### Remediation
Types: `Remediation`, `SolutionDetails`, `Exception`, `ExceptionDetails`

### Ticketing
Types: `Ticket`, `TicketStatus`

### InsightIDR (SIEM/XDR)
Types: `Alert`, `AlertRule`, `InsightIDR`, `Investigation`, `InvestigationStatus`, `Log`, `Ingestion`

### SOAR / InsightConnect
Types: `SOAR`, `SOARWorkflow`

### Platform
Types: `APIKey`, `Token`, `Webhook`

## Operations

### Queries
- `asset(id: ID!)`: Fetch a single asset by ID
- `assets(filter: AssetFilter, page: Int, size: Int)`: List assets with filtering
- `assetGroup(id: ID!)`: Fetch an asset group
- `assetGroups(page: Int, size: Int)`: List asset groups
- `vulnerability(id: ID!)`: Fetch vulnerability details
- `vulnerabilities(filter: VulnFilter, page: Int, size: Int)`: List vulnerabilities
- `scan(id: ID!)`: Fetch scan details
- `scans(siteId: ID, status: ScanStatus, page: Int, size: Int)`: List scans
- `site(id: ID!)`: Fetch site details
- `sites(page: Int, size: Int)`: List sites
- `report(id: ID!)`: Fetch report details
- `reports(page: Int, size: Int)`: List reports
- `investigation(id: ID!)`: Fetch InsightIDR investigation
- `investigations(status: InvestigationStatus, page: Int, size: Int)`: List investigations
- `alert(id: ID!)`: Fetch alert details
- `alerts(ruleId: ID, page: Int, size: Int)`: List alerts
- `policy(id: ID!)`: Fetch policy details
- `policies(page: Int, size: Int)`: List policies
- `exploit(id: ID!)`: Fetch exploit details
- `exploits(page: Int, size: Int)`: List exploits
- `credential(id: ID!)`: Fetch credential
- `credentials(page: Int, size: Int)`: List credentials
- `ticket(id: ID!)`: Fetch ticket
- `tickets(status: TicketStatus, page: Int, size: Int)`: List tickets
- `soarWorkflow(id: ID!)`: Fetch SOAR workflow
- `soarWorkflows(page: Int, size: Int)`: List SOAR workflows
- `apiKeys`: List API keys for current organization
- `webhooks(page: Int, size: Int)`: List webhooks

### Mutations
- `createScan(input: CreateScanInput!)`: Launch a new scan
- `stopScan(id: ID!)`: Stop an active scan
- `createSite(input: CreateSiteInput!)`: Create a new site
- `updateSite(id: ID!, input: UpdateSiteInput!)`: Update site configuration
- `deleteSite(id: ID!)`: Delete a site
- `createAssetGroup(input: CreateAssetGroupInput!)`: Create asset group
- `updateAssetGroup(id: ID!, input: UpdateAssetGroupInput!)`: Update asset group
- `deleteAssetGroup(id: ID!)`: Delete asset group
- `tagAsset(assetId: ID!, tag: AssetTagInput!)`: Tag an asset
- `untagAsset(assetId: ID!, tagKey: String!)`: Remove tag from asset
- `createException(input: CreateExceptionInput!)`: Create vulnerability exception
- `updateException(id: ID!, input: UpdateExceptionInput!)`: Update exception
- `deleteException(id: ID!)`: Delete exception
- `createReport(input: CreateReportInput!)`: Generate a report
- `deleteReport(id: ID!)`: Delete a report
- `createCredential(input: CreateCredentialInput!)`: Create scan credential
- `updateCredential(id: ID!, input: UpdateCredentialInput!)`: Update credential
- `deleteCredential(id: ID!)`: Delete credential
- `updateInvestigation(id: ID!, input: UpdateInvestigationInput!)`: Update IDR investigation status
- `createAlertRule(input: CreateAlertRuleInput!)`: Create IDR alert rule
- `updateAlertRule(id: ID!, input: UpdateAlertRuleInput!)`: Update alert rule
- `deleteAlertRule(id: ID!)`: Delete alert rule
- `createWebhook(input: CreateWebhookInput!)`: Register a webhook
- `updateWebhook(id: ID!, input: UpdateWebhookInput!)`: Update webhook
- `deleteWebhook(id: ID!)`: Delete webhook
- `triggerSOARWorkflow(id: ID!, input: SOARTriggerInput!)`: Trigger a SOAR workflow
- `createAPIKey(input: CreateAPIKeyInput!)`: Create an API key
- `deleteAPIKey(id: ID!)`: Delete an API key

## Source

Schema derived from:
- https://docs.rapid7.com/insight/api-documentation/
- https://help.rapid7.com/insightvm/en-us/api/api.html
- https://docs.rapid7.com/insightidr/api-overview/
- https://docs.rapid7.com/insight/api-overview/
