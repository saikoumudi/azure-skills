# Changelog

All notable changes to the Azure plugin will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/).

## [1.0.19] - 2026-04-16

### Changed

- Updated `azure-compute` skill: added VM quotas reference and enhanced VM recommender workflow.
- Updated `azure-quotas` skill: streamlined skill definition.
- Updated `microsoft-foundry` skill: updated foundry agent deployment documentation.

## [1.0.18] - 2026-04-15

### Added

- `azure-prepare`: added Static Web Apps references (deployment guide and Terraform).

### Changed

- Updated `azure-deploy` skill: expanded pre-deploy checklist, added Terraform error references, and enhanced azd error handling.
- Updated `azure-prepare` skill: improved .NET Aspire and azd Terraform documentation.
- Updated telemetry hook scripts.

## [1.0.17] - 2026-04-13

### Added

- `.cursor-plugin/plugin.json` — Cursor IDE plugin manifest.
- `hooks/cursor-hooks.json` — hooks configuration for Cursor.
- `assets/azure-logo.svg` — plugin logo asset.

### Changed

- Updated `gemini-extension.json`.

## [1.0.16] - 2026-04-13

### Changed

- Updated `azure-cost` skill: improved cost query guardrails, examples, and workflow; enhanced cost forecast guardrails.
- Updated `azure-prepare` and `azure-validate` skills.

## [1.0.15] - 2026-04-10

### Added

- `azure-kubernetes`: added AKS rightsizing, VPA, cluster autoscaler, and spot node pool reference files.
- `azure-validate`: added azd validation documentation.

### Changed

- Updated `azure-kubernetes` skill: expanded cost optimization scenarios with deep-dive references.
- Updated `azure-deploy` skill.
- Updated `azure-prepare` and `azure-validate` skills: improved functional and role verification references.

## [1.0.14] - 2026-04-09

### Added

- Root `gemini-extension.json` — Google Gemini CLI plugin manifest.

## [1.0.13] - 2026-04-09

### Added

- `gemini-extension.json` inside the plugin folder for Google Gemini CLI support.
- `azure-cloud-migrate`: added Cloud Run to Azure Container Apps migration and assessment guides.

### Changed

- Updated `azure-deploy` skill: refined pre-deploy checklist and error references.
- Updated `azure-prepare` skill: improved Container Apps Bicep and SQL Database references.

## [1.0.12] - 2026-04-08

### Added

- `azure-compute`: split VM troubleshooting into separate focused reference files (credential auth errors, firewall blocking, network connectivity, RDP connectivity, RDP service config, SSH connectivity, VM agent not responding).
- `azure-deploy`: added EF migration scripts (PowerShell and Bash) and SQL access grant scripts.
- `azure-prepare`: added SQL Database Bicep references and SQL access grant scripts.

### Changed

- Updated `azure-deploy` skill: refactored EF migrations documentation.
- Updated `azure-enterprise-infra-planner` skill.
- Updated `azure-hosted-copilot-sdk` skill.
- Updated `azure-prepare` skill: added App Service Bicep references.

## [1.0.11] - 2026-04-07

### Added

- `azure-deploy`: added pre-deploy checklist reference.
- `azure-prepare`: added .NET Aspire reference and expanded Aspire/azd guidance.

### Changed

- Updated `azure-deploy` skill: enhanced azd README with additional guidance.
- Updated `microsoft-foundry` skill: expanded troubleshoot and deploy documentation.

## [1.0.10] - 2026-04-06

### Added

- `azure-deploy`: added post-deployment verification, azd verify, EF migrations, Terraform README, and SQL managed identity references.
- `azure-prepare`: enhanced Container Apps Bicep references.

### Changed

- Updated `azure-deploy` skill: expanded error handling guidance.
- Updated `azure-hosted-copilot-sdk` skill.
- Updated `microsoft-foundry` skill: updated quota documentation.

## [1.0.9] - 2026-04-03

### Changed

- Updated `azure-hosted-copilot-sdk` skill: enhanced deployment guidance.
- Updated `azure-prepare` skill: improved App Service, .NET Aspire, architecture, research, and security references.
- Updated `entra-app-registration` skill.
- Updated `microsoft-foundry` skill: improved quota and capacity planning references.
- Updated telemetry hook scripts.

## [1.0.8] - 2026-04-02

### Added

- `azure-cost` — cost queries, cost forecasts, and cost optimization (replaces `azure-cost-optimization`).

### Removed

- `azure-cost-optimization` skill (functionality consolidated into `azure-cost`).

### Changed

- Updated `azure-deploy` skill: enhanced azd error handling and troubleshooting references.
- Updated `azure-prepare` skill: improved azd IaC rules and Bicep patterns.
- Updated `azure-resource-lookup` skill.

## [1.0.7] - 2026-04-01

### Added

- Telemetry hook scripts (`hooks/scripts/track-telemetry.sh` and `track-telemetry.ps1`).
- `hooks/hooks.json` and `copilot-hooks.json`.

### Changed

- Updated `azure-deploy` skill: added live role verification reference.
- Updated `azure-prepare` skill: added functional verification reference.
- Updated `azure-validate` skill: added role verification reference.

## [1.0.6] - 2026-03-31

### Added

- Root `.claude-plugin/plugin.json` — Claude Code plugin manifest at the repository root.

### Changed

- Updated `azure-deploy` skill: updated deployment recipes.
- Updated `azure-enterprise-infra-planner` skill: removed prescriptive mandatory language from the skill definition.
- Updated `azure-prepare` and `azure-validate` skills.

## [1.0.5] - 2026-03-30

### Added

- `azure-cost-optimization`: added AKS anomaly detection reference and AKS Cost Add-on reference.
- `azure-prepare`: added .NET Aspire reference.

### Changed

- Updated `azure-messaging` skill.
- Updated `azure-prepare` skill.

## [1.0.4] - 2026-03-27

### Changed

- Updated README with clarified Azure Kubernetes Service documentation.

## [1.0.3] - 2026-03-26

### Added

- `azure-prepare`: added App Service deployment slots documentation and enhanced Functions references (Bicep and Terraform).

### Changed

- Updated `azure-prepare` skill.

## [1.0.2] - 2026-03-25

### Added

- `azure-validate`: added validation recipe documentation (Azure CLI, azd, Bicep, Terraform).

### Changed

- Updated `azure-prepare` skill: improved functions templates, global rules, and plan template.
- Updated SQL Database authentication and Bicep references.

## [1.0.1] - 2026-03-13

### Added

- `azure-upgrade` — Assess and upgrade Azure workloads between plans, tiers, or SKUs.

### Changed

- Removed `foundry-mcp` HTTP server from `.mcp.json` (non-spec `type`/`url` fields).
- Updated `azure-diagnostics` description.
- Updated `microsoft-foundry` description and bumped to version 1.0.5.

## [1.0.0] - 2025-03-12

### Added

- Initial release of the Azure plugin.
- Vendor-neutral `.plugin/plugin.json` manifest following the [Open Plugins Specification](https://open-plugins.com/plugin-builders/specification).
- Claude Code manifest (`.claude-plugin/plugin.json`).
- MCP server configuration (`.mcp.json`) for Azure MCP, Foundry MCP, and Context7.
- MIT `LICENSE` file at the plugin root.
- 21 agent skills:
  - `appinsights-instrumentation` — Azure Application Insights telemetry setup.
  - `azure-ai` — Azure AI Search, Speech, OpenAI, and Document Intelligence.
  - `azure-aigateway` — Azure API Management as an AI Gateway.
  - `azure-cloud-migrate` — Cross-cloud migration assessment and code conversion.
  - `azure-compliance` — Security auditing and best practices assessment.
  - `azure-compute` — VM size recommendation and configuration.
  - `azure-cost-optimization` — Cost savings analysis and recommendations.
  - `azure-deploy` — Azure deployment execution (azd, Bicep, Terraform).
  - `azure-diagnostics` — Production issue debugging and log analysis.
  - `azure-hosted-copilot-sdk` — Build and deploy GitHub Copilot SDK apps to Azure.
  - `azure-kusto` — Azure Data Explorer KQL queries.
  - `azure-messaging` — Event Hubs and Service Bus SDK troubleshooting.
  - `azure-prepare` — Application preparation for Azure deployment.
  - `azure-quotas` — Quota and usage management.
  - `azure-rbac` — RBAC role recommendation and assignment.
  - `azure-resource-lookup` — Azure resource discovery and listing.
  - `azure-resource-visualizer` — Mermaid architecture diagram generation.
  - `azure-storage` — Blob, File, Queue, Table, and Data Lake storage.
  - `azure-validate` — Pre-deployment validation checks.
  - `entra-app-registration` — Microsoft Entra ID app registration and OAuth setup.
  - `microsoft-foundry` — Foundry agent deployment, evaluation, and management.