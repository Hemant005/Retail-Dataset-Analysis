# 🛒 Retail Data Warehouse Project

## 📌 Overview

This project demonstrates a cloud-based retail data pipeline using **AWS Services**. It automates the ingestion, transformation, storage, and visualization of retail sales data for reporting and analytics purposes.

---

## 🧱 Architecture

1. **Input S3 Bucket**  
   Raw retail CSV files are uploaded here.

2. **AWS Lambda**  
   Acts as a trigger for every new file uploaded to the input S3 bucket.

3. **AWS Glue Job**  
   Processes and transforms the raw CSV data into a structured **Parquet** format.

4. **Output S3 Bucket**  
   Stores the transformed parquet files.

5. **Amazon Redshift**  
   Serves as the data warehouse. The processed data is loaded from the output S3 bucket into Redshift for analytics and reporting.

6. **Power BI**  
   Connected to Redshift (using Redshift ODBC or Athena ODBC) to visualize sales data through interactive dashboards.

---

## 🔧 Tools & Services Used

- **AWS S3** – Storage for raw and processed files  
- **AWS Lambda** – Event-driven trigger for Glue jobs  
- **AWS Glue** – ETL (Extract, Transform, Load) job  
- **Amazon Redshift** – Cloud data warehouse  
- **Power BI** – Visualization and reporting

---

## 🎯 Key Features

- End-to-end serverless ETL pipeline
- Automatic job trigger on new data
- Scalable and cost-effective warehouse solution
- Integration with BI tools for real-time insights

---

## 🚀 Future Improvements

- Add data partitioning in Glue for performance
- Include error handling & logging in Lambda
- Automate Redshift loading via AWS Glue jobs or Lambda
- Explore scheduling using **Amazon EventBridge**

---
