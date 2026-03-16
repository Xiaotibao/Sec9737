# Sec9737
API Security - Feature Overview
API Security is an API security scanning solution built on OpenSCA, Semgrep, and afrog. It helps teams find and fix API vulnerabilities across dependencies, code, and runtime.

Core Detection
The tool covers OWASP API Top 10 risks, including broken object-level authorization, broken authentication, excessive data exposure, and unsafe consumption of APIs. It combines:

OpenSCA for dependency CVE scanning
Semgrep for static code analysis
afrog for dynamic API scanning
Custom rules for project-specific checks
It supports OpenAPI 2.0 and 3.0, auto-detects OpenAPI/Swagger files, and performs compliance checks (e.g., missing security definitions, sensitive field exposure, missing 401/403). An incremental scan mode scans only git-changed files to speed up CI.

Admin Dashboard
A web dashboard provides:

Statistics on scan counts and vulnerability severity
Finding filters by API, severity, and tool
Trend charts for 7/30-day vulnerability trends
Member management for team access
Critical summary for high-severity issues
Scan triggers with progress tracking
Export to Excel/PDF
Data cleanup with configurable retention
Audit logs for operations
Webhooks for Feishu, Slack, DingTalk, WeCom, or custom endpoints
API change analysis by comparing old and new OpenAPI specs
Custom rules with 24 built-in rules that can be enabled or disabled
AI & Integrations
AI repair suggestions in finding details, with patch drafts (LLM or static templates)
VS Code extension for workspace scanning and a Problems panel
GitHub Actions templates for basic and advanced workflows
GitLab CI and Jenkins integration with MR/PR incremental scanning
Editions
The Community Edition (default) is free and open source, with no billing or team limits. The Enterprise Edition adds plan-based billing, multi-tenancy, and SSO.
