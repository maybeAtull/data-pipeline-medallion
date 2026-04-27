**#Project Description **
Designed and implemented an end-to-end data pipeline using Medallion Architecture (Bronze, Silver, Gold) for scalable and structured data processing
Developed an API ingestion pipeline to extract data and store it in the Bronze layer (Delta format) with ingestion timestamps for traceability
Built a Silver layer transformation pipeline with:
Data type casting and cleansing
Reusable Data Quality framework
Segregation of good and bad records with rejection reasons
Implemented incremental data processing using watermarking, ensuring only new data is processed, improving efficiency and scalability
Used Delta Lake MERGE (upsert) operations to maintain idempotency and avoid duplicate data
Created a quarantine layer to store invalid records for debugging and audit purposes
Developed a Gold layer to generate aggregated, business-ready datasets for analytics and reporting
Orchestrated the pipeline using Databricks Workflows, scheduling jobs to run sequentially (Bronze → Silver → Gold)
Integrated email alerting system to notify on pipeline success/failure, improving operational reliability
Built a pipeline monitoring system:
Logged execution details in pipeline_runs table
Tracked records processed, bad records, and run status
Designed a Power BI dashboard featuring:
KPI cards (Total Runs, Records Processed, Bad Records, Success Rate)
Trend analysis of data quality (Good vs Bad records)
Pipeline health monitoring over time
