Integrated Operations Analysis

📊 Manufacturing Operations Analytics + Automation (SQL, Excel, Power BI, n8n, GenAI)

An end-to-end data analytics and automation project built on a manufacturing dataset to analyze operations, generate insights, and automate reporting using n8n + GenAI for real-time decision-making.

🚨 Problem Statement

Manufacturing companies struggle with managing large volumes of operational data across shipments, payments, customers, and employees. This leads to:

Inefficient manual reporting and delayed insights
Lack of real-time visibility into operations
Difficulty in identifying bottlenecks in shipments and payments
⚙️ Workflow Steps
1. ⏰ Schedule Trigger

Fires automatically every day at 8:00 AM using n8n's built-in cron scheduler.

2. 📥 HTTP Request — Fetch CSV

Fetches the latest logistics data from a static CSV file hosted on Google Drive using a direct download URL.

3. 🔧 Code Node — Parse & Structure Data

Parses the raw CSV into a clean JSON format and calculates:

Delivery rate (%) per segment
Not delivered count per segment
Total pending payments
4. 🤖 Basic LLM Chain — Groq AI Summary

Sends structured data to Groq (LLaMA3-70b) with a prompt that:

Flags critical non-delivery rates (>20%)
Links COD pending payments to undelivered shipments
Identifies the worst-performing segment
Generates actionable recommendations
5. 📧 Gmail — Send Report

Sends a formatted HTML email to the operations team with:

Data snapshot table
AI-generated summary
📸 Screenshots
🔹 n8n Workflow
<p align="center"> <img src="https://github.com/user-attachments/assets/c49d4fe8-ae0e-46b5-a4c9-7f41f5623561" width="800"> </p>
🔹 Automated Report Output
<p align="center"> <img src="https://github.com/user-attachments/assets/e9c0cdac-eb0c-4367-9352-633bea2d4c6f" width="500"> </p>

🛠️ Tech Stack

Tool	Purpose
n8n	Workflow automation
Groq (LLaMA3-70b)	AI summary generation
Google Drive	CSV data hosting
Gmail	Report delivery

🚀 How to Run

Import workflow/logistics_report.workflow.json into n8n
Set up credentials — Groq API key + Gmail OAuth
Upload your CSV to Google Drive
Update the HTTP Request URL with your file link
Activate the workflow — report runs daily at 8AM

👤 Author

Siddhant Pagare
