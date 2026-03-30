DA05-Integrated-Operations-Analysis

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

Parses the raw CSV key-value format into a clean JSON object and calculates:

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
n8n Workflow

<img width="1277" height="516" alt="objective 1 workflow" src="https://github.com/user-attachments/assets/c49d4fe8-ae0e-46b5-a4c9-7f41f5623561" />

Automated Report Output

<img width="576" height="620" alt="objective 1 output" src="https://github.com/user-attachments/assets/e9c0cdac-eb0c-4367-9352-633bea2d4c6f" />


🛠️ Tech Stack
Tool	Purpose
SQL (PostgreSQL/Colab)	Data extraction & transformation
Excel	Data cleaning & EDA
Power BI	Dashboard & visualization
n8n	Workflow automation
GenAI (LLM)	Automated summaries & explanations
🚀 How to Run
Load datasets into SQL and perform ETL
Export cleaned data to Excel for analysis
Build Power BI dashboard using processed data
Set up n8n workflows:
Add data source (CSV/SQL)
Configure GenAI API
Set triggers (cron/webhook)
Activate workflows for automated reporting
<img width="576" height="620" alt="objective 1 output" src="https://github.com/user-attachments/assets/61b259e1-a3e9-457b-8ced-5fbd24698005" />

🎯 Conclusion
Reduced manual reporting effort by ~35–40%
Enabled real-time insights and automated decision support
Improved operational efficiency and visibility across logistics and payments
👤 Author
Siddhant Pagare
