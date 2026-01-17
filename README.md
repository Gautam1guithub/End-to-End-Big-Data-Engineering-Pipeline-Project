# End-to-End-Big-Data-Engineering-Pipeline-Project
An end-to-end big data engineering pipeline built on AWS, leveraging EMR and Apache Spark for large-scale data processing, S3 for scalable storage, and Redshift Serverless for analytics-ready data validation and querying.
# Architecture Flow
Local System → S3 → EMR (Spark) → S3(Transformed data) → Redshift Serverless
# Step 1: EMR Cluster Creation
<img width="1893" height="807" alt="EMR project(1)" src="https://github.com/user-attachments/assets/a091d2df-3176-4fa0-9538-3400732a9eda" />


# Step 2: EMR Remote Development & Cluster Access Configuration
Configured secure remote access to the EMR cluster for Spark application development and execution.
<img width="1918" height="987" alt="EMR project(2)" src="https://github.com/user-attachments/assets/afd68a96-3369-4d8e-9237-96aa57c3386f" />
<img width="1918" height="1017" alt="EMR project(3)" src="https://github.com/user-attachments/assets/855fda0b-c83a-4e08-ada5-f6ef93a22076" />


# Step 3: GitHub Archive Data Ingestion
Downloaded GitHub Archive event data for large-scale analytical processing.
<img width="1920" height="1080" alt="EMR(12)" src="https://github.com/user-attachments/assets/04c75a7a-f1e6-4185-b0d2-da926409793b" />


# Step 4: Raw Data Storage in Amazon S3
Uploaded raw datasets to Amazon S3 for durable, scalable, and cost-effective storage.
<img width="1920" height="926" alt="EMR(13)" src="https://github.com/user-attachments/assets/0c7b7093-f733-473b-af53-4f453bcc9877" />



# Step 5: Distributed Data Reading with Apache Spark
Read raw data from S3 into Spark DataFrames for distributed processing.


# Step 6: Data Cleaning and Transformation
Performed data cleansing, filtering, and transformations using Spark SQL and DataFrame APIs.
<img width="1920" height="1080" alt="EMR(14)" src="https://github.com/user-attachments/assets/0b867bf3-926d-483b-808e-cfc149fd09c9" />


# Step 7: Transformed Data Persistence to S3 (Staging Layer)
Stored transformed and intermediate datasets in a temporary S3 staging location using optimized formats.
<img width="1920" height="925" alt="EMR(15)" src="https://github.com/user-attachments/assets/dd215d2e-8080-436a-860e-8593e74ccaf8" />


# Step 8: Amazon Redshift Serverless Environment Setup
Configured Redshift Serverless by creating the required namespace and workgroup.
<img width="1888" height="851" alt="EMR project(7)" src="https://github.com/user-attachments/assets/4bf5240d-e2ba-40a2-b21a-1c43015769a3" />


# Step 9: Analytical Table Design and Creation in Redshift
Designed and created Redshift tables optimized for analytical workloads.
<img width="1918" height="871" alt="EMR project(8)" src="https://github.com/user-attachments/assets/663f7312-8aa7-4ee9-9e48-054289b2c758" />


# Step 10: Data Loading into Redshift via Spark Integration
Loaded transformed data from S3 into Amazon Redshift using Spark JDBC integration.
![EMR(18) png](https://github.com/user-attachments/assets/5474b88e-0198-4562-9782-3b1192a26d88)
![EMR(19) png](https://github.com/user-attachments/assets/005da560-cc0d-4898-b7ff-b7f05f35b7c6)


# Step 11: Data Quality Validation and Consistency Checks
Validated record counts, schema alignment, and data quality within Redshift.
<img width="1920" height="916" alt="EMR(17)" src="https://github.com/user-attachments/assets/f67d0012-d8ba-4121-8f0e-5d34be98cd4c" />
