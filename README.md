# Bronze-Silver-Gold-ETL-Pipeline
This project demonstrates an end-to-end data pipeline for e-commerce data using the Medallion Architecture, which consists of three layers: Bronze, Silver, and Gold.
In the Bronze layer, raw data from various sources is ingested and stored in its original form for traceability and auditing.
The data then flows into the Silver layer, where it undergoes cleansing and transformation based on business requirements. This includes handling null values, removing duplicates, and standardizing formats.
Finally, the curated data is moved to the Gold layer, where it is modeled into fact and dimension tables. A denormalized reporting table is also created, which serves as a single source of truth for downstream teams involved in reporting, analytics, and machine learning use cases.
Since e-commerce platforms generate data on a daily basis, this pipeline is designed to support incremental loading, ensuring that new records are seamlessly merged with historical data to maintain a complete and up-to-date dataset.
