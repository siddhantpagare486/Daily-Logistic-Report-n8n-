DA05-Integrated-Operations-Analysis

📊 Manufacturing Operations Analytics + Automation (SQL, Excel, Power BI, n8n, GenAI)

An end-to-end data analytics and automation project built on a manufacturing dataset to analyze operations, generate insights, and automate reporting using n8n + GenAI for real-time decision-making.

🚨 Problem Statement

Manufacturing companies struggle with managing large volumes of operational data across shipments, payments, customers, and employees. This leads to:

Inefficient manual reporting and delayed insights
Lack of real-time visibility into operations
Difficulty in identifying bottlenecks in shipments and payments

This project solves these challenges by combining data analytics + dashboards + AI automation to deliver actionable insights and automated reporting.

⚙️ Workflow Overview
1. 📥 Data Extraction (SQL ETL)
Loaded multiple datasets (Customer, Shipment, Payment, Employee, Status) into SQL
Performed data cleaning, normalization, and transformations
2. 🔧 Data Processing & Analysis (Excel)
Handled missing values and duplicates
Performed EDA to identify trends in shipments, payments, and customer behavior
Created calculated fields like payment categories and shipment efficiency
3. 📊 Dashboarding (Power BI)

Built an interactive dashboard including:

Customer segmentation and insights
Employee performance tracking
Shipment analysis (Domestic vs International, Express vs Regular)
Financial overview (payments, pending amounts, trends)
4. 🤖 Automation (n8n + GenAI)
✅ Workflow 1: Daily Operations Summary
Triggered daily using cron
Fetches aggregated metrics
Uses GenAI to generate a simple summary
Sends report via email/Slack
✅ Workflow 2: AI Issue Explanation System
Takes Shipment ID / Customer ID as input
Fetches related data
Uses GenAI to explain delays or payment issues in plain language
🤖 GenAI Usage
Input
Shipment metrics
Payment status
Employee handling data
Customer & membership details
Output
Daily automated summaries
AI-based explanations for delays and payment issues
Example Output

“Shipment SH_1023 is delayed due to international transit time. Payment is pending as it is COD and delivery is incomplete. The assigned employee is managing multiple international shipments, contributing to the delay.”

📊 Key Insights
Most shipments fall under 80–100 kg category impacting cost
Domestic shipments have higher delivery success rates
COD payments are a major contributor to pending revenue
Certain employees handle disproportionately higher workloads
📸 Screenshots
Power BI Dashboard
n8n Workflow
Automated Report Output

(Add images here in your GitHub repo)

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
🎯 Conclusion
Reduced manual reporting effort by ~35–40%
Enabled real-time insights and automated decision support
Improved operational efficiency and visibility across logistics and payments
👤 Author

Siddhant Pagare
