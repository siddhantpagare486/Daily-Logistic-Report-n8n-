# 🚀 Integrated Operations Analysis

## 📊 Manufacturing Operations Analytics + Automation</b><br> (SQL, Excel, Power BI, n8n, GenAI) 

### 📌 Project Overview

An end-to-end data analytics + automation project built on a manufacturing dataset to:

Analyze operational performance
Generate actionable insights
Automate reporting using n8n + GenAI

👉 Designed to simulate real-world business decision systems used in modern companies.

### 🚨 Problem Statement

Manufacturing operations face major challenges due to fragmented data across shipments, payments, customers, and employees:

⏳ Manual reporting → time-consuming & error-prone
📉 No real-time visibility into operations
⚠️ Difficulty identifying bottlenecks in logistics & payments

💡 Goal: Build a system that converts raw data into automated insights + intelligent reports.

### ⚙️ End-to-End Workflow
🔹 1. Schedule Trigger

⏰ Runs daily at 8:00 AM using n8n cron

🔹 2. Data Ingestion

📥 Fetches logistics data from Google Drive (CSV)

🔹 3. Data Processing

🔧 Parses CSV → structured JSON

Delivery rate per segment
Not delivered counts
Pending payments
🔹 4. AI Analysis (GenAI)

🤖 Uses Groq (LLaMA3-70B) to:

Detect critical issues (>20% failure)
Link COD pending to undelivered shipments
Identify worst-performing segment
Generate recommendations

🔹 5. Automated Reporting

📧 Sends AI-generated report via Gmail

Data snapshot
Business insights
Actionable suggestions
📸 Project Preview
🔹 n8n Workflow
<p align="center"> <img src="https://github.com/user-attachments/assets/c49d4fe8-ae0e-46b5-a4c9-7f41f5623561" width="850"> </p>
🔹 AI Generated Report
<p align="center"> <img src="https://github.com/user-attachments/assets/e9c0cdac-eb0c-4367-9352-633bea2d4c6f" width="500"> </p>
🧠 GenAI Intelligence
📥 Input
Shipment metrics
Payment data
Segment breakdown
Delivery performance

### ⚡ Output
Automated daily summaries
Bottleneck detection
Smart recommendations

### 💬 Sample Insight:

“Domestic Express shipments show critical delays (>20% failure). COD payments are pending due to undelivered shipments. Immediate operational intervention required.”

### 🛠️ Tech Stack
Category	Tools
Data Processing	SQL, Excel
Visualization	Power BI
Automation	n8n
AI	Groq (LLaMA3-70B)
Data Source	Google Drive
Delivery	Gmail
🚀 How to Run
 1. Import workflow into n8n
 2. Add credentials (Groq API + Gmail)
 3. Upload CSV to Google Drive
 4. Update HTTP request URL
 5. Activate workflow

### 📌 Workflow will run automatically every day at 8:00 AM

📈 Business Impact
⚡ Reduced manual reporting by 35–40%
📊 Improved real-time decision-making
🔍 Faster issue detection in logistics
🤖 Enabled AI-driven operations
🎯 Key Highlights

✔ End-to-end data pipeline (ETL → Dashboard → Automation)
✔ Real-world business problem solving
✔ GenAI integration for intelligent insights
✔ Production-style automation workflow

👤 Author

Siddhant Pagare

📧 siddhantpagare913@gmail.com
