Care Connect Health Network – Healthcare Data Engineering Project

Built an end-to-end healthcare data platform using Azure Data Factory and Databricks to collect and process data from multiple hospitals and external partners.

The project uses a metadata-driven approach, where a single reusable ADF pipeline handles data ingestion based on configurations stored in a SQL control table. Data is processed through Bronze, Silver, and Gold layers using Databricks and Delta Lake.

Key Features:

Automated data ingestion from PostgreSQL, CSV files, and Azure SQL.
Supports full and incremental data loads.
Built Bronze, Silver, and Gold layers using Databricks.
Used PySpark and SQL for data cleaning and transformation.
Implemented data auditing, logging, and email notifications.
Used Unity Catalog, Managed Identity, and Azure Key Vault for security.
Set up CI/CD using GitHub for ADF and Databricks.
Created dashboards and Genie Agents for reporting and data insights.

Technologies: Azure Data Factory, Azure Databricks, PySpark, Python, SQL, Delta Lake, Unity Catalog, ADLS Gen2, Azure Key Vault, Logic Apps, GitHub, and Databricks AI/BI.
