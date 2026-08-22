# 📊 careplus-support-tickets-logs-etl-pipeline
This project demonstrates an end-to-end ETL pipeline for CarePlus Support Data. The pipeline ingests support tickets (CSV) and system logs, transforms them using AWS Glue & Lambda, and stores them in Amazon Redshift Spectrum for analytics and reporting.

## 🚀 Project Architecture
The pipeline integrates S3, Lambda, Glue, and Redshift Spectrum into a seamless flow:

<img width="1202" height="737" alt="image" src="https://github.com/user-attachments/assets/9e4f47b1-a988-4c66-8024-7bbb6b49a68a" />

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🔹 Log Data Pipeline
* Source: Raw support logs (unstructured .log files)
* Processing: AWS Lambda function (lambda_log_etl.py) parses and transforms logs into a structured format
* Target: Transformed logs stored in S3 and queried via Redshift Spectrum

 ### Architecture

<img width="1635" height="447" alt="image" src="https://github.com/user-attachments/assets/500aa8ba-a766-4731-8ef5-50cb0ce3584e" />


 ### Insights

 <img width="1238" height="702" alt="image" src="https://github.com/user-attachments/assets/e73e46e3-2ab4-4399-977a-1c5779fb3ea7" />

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### 🔹 Ticket Data Pipeline

* Source: Support ticket CSV files (daily ingestions)
* Processing: AWS Glue ETL job (glue_ticket_etl.py) cleans and standardizes data
* Target: Transformed tickets stored in S3 and queried via Redshift Spectrum

 <img width="1630" height="513" alt="image" src="https://github.com/user-attachments/assets/d22db56f-060a-42cb-88a6-0938c9fe9075" />

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

📂 Repository Structure

<img width="835" height="281" alt="image" src="https://github.com/user-attachments/assets/30d476c4-c6ff-4032-9bb4-47add2122a72" />

## ⚙️ Tech Stack

* AWS Lambda → ETL for log files
* AWS Glue → ETL for support tickets (CSV)
* Amazon S3 → Storage (Raw & Processed Zones)
* Amazon Redshift Spectrum → Query engine for analytics
* Visualization → Insights dashboards (BI tool)

## 📌 Key Learnings
✅ Building ETL pipelines with AWS services 

✅ Handling structured (CSV) & unstructured (logs) data 

✅ Designing scalable data lake → warehouse architecture 

✅ Visualizing insights from Redshift queries

## 📬 Contact

Feel free to reach out if you have any questions or would like to connect!

[📧 Gmail](mailto:connectingsrl@gmail.com)  
[🔗 LinkedIn](https://www.linkedin.com/in/sahajahanur-laskar/)









 

