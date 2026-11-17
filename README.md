Care Connect Health Network — Metadata-Driven Healthcare Data Platform | Azure Data Factory | Databricks | Unity Catalog

An end-to-end, metadata-driven data engineering project for a multi-hospital healthcare network. It ingests relational data from an internal hospital system (PostgreSQL) alongside recurring file-based feeds from external partners (CSV), then transforms everything through a Bronze–Silver–Gold medallion architecture on Databricks — all driven by a single reusable Azure Data Factory pipeline configured entirely from a SQL control table, with every run automatically audited and reported by email.

Key Features
Metadata-driven ingestion — a single Azure Data Factory pipeline ingests every source, relational or file-based, based on rows in a SQL control table. Onboarding a new source means adding a row, not writing a new pipeline.
Full and incremental loads — full-reload, append, and watermark-based merge load strategies, all handled by the same generic notebooks.
Bronze–Silver–Gold medallion architecture — raw, standardized, and curated reporting layers on Delta Lake, with a supporting calendar dimension table.
Automated auditing & alerting — every stage of every run is logged, and a status email (with a dynamic subject and an HTML results table) goes out automatically via Azure Logic Apps, whether the run succeeds or fails.
Governed, credential-less storage access — Unity Catalog storage credentials and managed identities throughout; no account keys or passwords in any pipeline definition.
CI/CD for both platforms — feature-branch and pull-request workflows for Azure Data Factory and Databricks Repos alike.
Multiple consumption surfaces — a multi-page Databricks dashboard, a scoped Genie Agent, and a workspace-wide Genie ONE natural-language interface, all built on the same gold tables.

1- Orchestration & Ingestion: Azure Data Factory, metadata-driven pipeline design, full & incremental (watermark) loads

2- Data Platform & Storage: Databricks, Delta Lake, Unity Catalog, Medallion Architecture, ADLS Gen2

3- Data Sources: PostgreSQL, file-based partner feeds, Azure SQL Database

4- Transformation: PySpark, Spark SQL, Delta Lake MERGE INTO, window functions, dimensional modeling

5- Governance & Security: Azure Key Vault, managed identity & role-based access control, credential-less storage access

6- Automation & Alerting: Azure Logic Apps, metadata-driven audit logging, automated email notifications

7- CI/CD: GitHub (Azure Data Factory & Databricks Repos), feature-branch/PR workflow

8- Consumption & BI: Databricks AI/BI Dashboards, Genie Agents, Genie ONE

9- Programming & Tooling: Python, PySpark, SQL, AI-assisted development
