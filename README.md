# Azure File Ingestion Pipeline using ADF

This project ingests three different file types from Azure Data Lake and loads them into Azure SQL tables using transformations based on filename patterns.

##  Pipeline Features:

- Supports three files: `CUST_MSTR`, `master_child_export`, `H_ECOM_ORDER`
- Extracts `date` and `dateKey` from filenames
- Performs truncate-load into SQL tables
- Daily scheduled trigger (or manual run)
- Uses wildcard + dynamic datasets

## Scheduling :

- Trigger Type: Schedule
- Time: Daily at 12:03 AM (custom tested time was 18:29 IST)

##  Output Verification :

- Files processed from ADLS
- SQL tables loaded with transformed data
- Monitor tab run succeeded

---
Author: 
Samiksha Kharche  

