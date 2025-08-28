# Automated Finance Reporting Workflow
This project is a make.com workflow designed to automate the generation and distribution of financial reports for a real estate business. It connects multiple data sources and services to produce clear, professional reports without manual intervention.
# Features
-	Multi-Report Generation:
○ Automatically creates comprehensive financial reports for three key areas:
○	Real Estate Property Performance
○	Employee Salaries and Payroll
○	Client Payments and Overdue Accounts
- AI-Powered Analysis: Utilizes OpenAI's GPT-4o to analyze raw data, identify key metrics, and generate well-structured reports in a professional, ready-to-share format.
- Seamless Integration: Connects Airtable as the primary data source and Google Drive for cloud-based file storage. Reports are automatically saved and linked within the Airtable database for easy access.
- Automated Distribution: Sends email notifications to key stakeholders with the final report, ensuring timely communication and data-driven decision-making.
# How It Works
1.	Trigger: The workflow is activated by a webhook, allowing for on-demand report generation.
2.	Data Retrieval: It queries three separate Airtable bases (Properties, Employees, and Clients) to gather the necessary financial data.
3.	Data Aggregation: The data for each report type is aggregated into a single bundle.
4.	AI Processing: The aggregated data is sent to the OpenAI API, which analyzes it and generates a detailed report based on a pre-defined prompt.
5.	File Management: The Markdown report is uploaded to a designated Google Drive folder.
6.	Database Update & Notification: The Airtable record is updated with a link to the new report, and an email is sent to the relevant recipients.
