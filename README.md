Project Title:
Data Quality Control for the City of Vancouver Using AWS

Project Description:
This project simulates the migration of the City of Vancouver's public data systems to a cloud-based analytics platform on AWS. The goal is to create a scalable, secure, and automated Data Analytics Platform (DAP) that enables data processing, quality checks, storage, monitoring, and visualization.

Objective:
To design and implement a cloud-native data analytics pipeline that can:

Ingested raw data securely

Applied automated data quality checks

Separatedvalid and invalid data

Monitored system performance and data flow

Visualize key metrics using dashboards

Dataset:
Issued Operating Permits for Water Systems – Sample dataset simulating real-world environmental permit data. The data was uploaded to an AWS S3 bucket as the raw input for the pipeline.

Methodology:

1.Secure Storage Setup:

Used AWS KMS to encrypt the raw data bucket (issued-operating-permits-watersystems-vai)

Enabled versioning for recovery and audit purposes ![Image](https://github.com/user-attachments/assets/cbe63b8c-c9dd-462d-a822-50089c083574)

2.ETL and Data Quality Checks: ![Image](https://github.com/user-attachments/assets/c23d4171-3084-4149-8200-9f7753f5ed40)

Built a visual ETL job using AWS Glue 

Created rules to validate incoming records

Stored passed records in watersystm-cln-vai/Pass/ and failed ones in watersystm-cln-vai/Fail/ ![Image](https://github.com/user-attachments/assets/20743f09-8bb1-4eeb-aa0e-4113463fbd80)
![image](https://github.com/user-attachments/assets/544aefb4-700e-4e72-867c-2e253b7103bd)


3.Monitoring and Alerts:

Configured AWS CloudWatch to track S3 bucket size and set alarms for thresholds

Used AWS CloudTrail to audit account activity
![Image](https://github.com/user-attachments/assets/db91ef94-d439-4c02-a142-598a0a5f8a91)
4.Dashboard Creation:




Tools and Technologies:-

Cloud Provider: AWS

Storage: Amazon S3

ETL Tool: AWS Glue (Visual ETL Jobs)

Security: AWS KMS

Monitoring: AWS CloudWatch, AWS CloudTrail

Visualization: AWS Glue

Others: IAM for role and policy management

Deliverables:

A secured and versioned S3 raw data bucket

An automated ETL pipeline with data quality validation

Organized S3 folders for pass/fail results

Monitoring dashboard with real-time alerts


