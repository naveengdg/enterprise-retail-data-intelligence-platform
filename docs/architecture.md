# System Architecture Flow


1. Data Sources

Instacart Dataset + Synthetic Data


        ↓


2. Ingestion

Azure Data Factory performs scheduled incremental loading


        ↓


3. Data Lake

ADLS Gen2 stores Bronze/Silver/Gold layers


        ↓


4. Processing

Databricks + PySpark performs transformations


        ↓


5. Warehouse

Snowflake stores analytics-ready data


        ↓


6. Intelligence Layer

LangGraph GenAI agent enables natural language analytics
