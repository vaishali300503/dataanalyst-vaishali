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

Enabled versioning for recovery and audit purposes

2.ETL and Data Quality Checks:

Built a visual ETL job using AWS Glue 

Created rules to validate incoming records

Stored passed records in watersystm-cln-vai/Pass/ and failed ones in watersystm-cln-vai/Fail/

3.Monitoring and Alerts:

Configured AWS CloudWatch to track S3 bucket size and set alarms for thresholds

Used AWS CloudTrail to audit account activity

4.Dashboard Creation:

Visualized processed data using Amazon QuickSight (or other dashboard tool if different)

Displayed key metrics like volume of passed vs failed records, bucket growth, etc.

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


