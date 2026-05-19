# fmcg-analytics-pipeline
Databricks pipeline for an FMCG acquisition. Ingests raw subsidiary data from AWS S3 into Delta Lake, standardizing disparate schemas and types via try_to_date and SHA-256 keys. Employs Window Functions to deduplicate batch data before executing an idempotent MERGE.
