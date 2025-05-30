MarketFlash: Marketing Campaign Database & Dashboard

🌍 About the Project

MarketFlash is a fictional marketing company owned by Markus, who originally stored all business data in a single spreadsheet. This project was created to redesign and structure that data by:

Building a relational database to organize campaigns, clients, employees, and related entities

Creating and importing cleaned, normalized tables into Google BigQuery

Designing interactive dashboards in Tableau for data exploration and reporting

This project demonstrates data modeling, SQL querying, data cleaning, and dashboard development skills using real-world scenarios.

📅 Business Case

Markus needed a more structured, scalable system to:

Eliminate redundancy and errors in his spreadsheet

Prepare for growth by including additional entities (influencers, payments, etc.)

Generate insightful visuals and reports to make data-driven decisions

🔢 Tools & Technologies Used

Google Sheets: Initial data cleaning, formatting, and table creation

DrawSQL: ER diagram design and data modeling

BigQuery: SQL database creation and querying

Apps Script: Custom script to clean incorrectly formatted phone numbers

Tableau: Dashboard development and presentation

📊 Dataset Overview

The original spreadsheet included fields such as:

Campaign Number, Campaign Name, Start/End Dates

Channel, Client, Audience, Location

Views, Likes, Clicks, Conversions, Expense

Executive contact person

Normalized Entities Created

Campaigns (ID, Name, StartDate, EndDate, Budget)

Clients (CompanyName, Address, Email, Phone#, ContactPerson)

Employees (EmpID, Name, Email, Supervisor)

Platforms (Platform_ID, Name, URL, Contact)

Influencers, Contents, Payments, Metrics, Advertisements

Relationships

One client can run many campaigns

Each campaign is managed by one employee

Each campaign may involve multiple platforms and influencers

One set of metrics per campaign

One or more ads and pieces of content per campaign

Ads tied to both platforms and campaigns

📃 Process

ER Diagram Design: Created in DrawSQL based on initial spreadsheet

Normalization: Functional model prepared with clean, linked tables

Data Cleaning:

Fixed trailing zeroes in date fields

Standardized phone number formats (resolved formula error using Apps Script)

Removed duplicate clients (e.g., Cli_026 and Cli_055)

Estimated missing budget values using Expense * 1.25

Data Import:

Created mock data for new tables where necessary

Imported from Google Sheets into BigQuery

Added dummy integers for import compatibility where all columns were originally strings

SQL Practice:

Wrote sample queries for campaign metrics, client performance, and employee involvement

Dashboards:

Campaign & Client Dashboard

Metrics Dashboard (views, conversions, expenses)

Employee Dashboard

Presentation:

Recorded a 5-minute video walkthrough for Markus summarizing key insights

📊 Key Takeaways

Improved Data Structure: Markus now has a scalable relational model to support growth

Clearer Insights: Dashboards highlight campaign effectiveness and employee/client performance

Future-Proofing: Extra entities (influencers, content, payments) make the system ready for expansion

✨ What I Learned

ER diagramming and normalization in DrawSQL

Data cleaning techniques in Sheets and Apps Script

Importing structured data into BigQuery

SQL joins and queries for campaign insights

Tableau dashboard design for different stakeholders

📢 Project Status

Completed – potential next steps:

Add user authentication for data access

Automate data pipeline using scheduled queries or integrations

Integrate campaign performance prediction using machine learning

🔍 File Structure (Example)

MarketFlash/
├── assets/                # Screenshots or Tableau exports
├── data/
│   ├── original_data.xlsx
│   ├── cleaned_data.csv
│   └── mock_data/
├── SQL/
│   ├── create_tables.sql
│   └── sample_queries.sql
├── dashboards/
│   └── tableau_links.txt
├── README.md
└── presentation/
    └── marketflash_pitch.mp4

👥 Author

Your NameData Analyst | SQL | Tableau | BigQuery | Excel

Feel free to connect with me on LinkedIn or explore my other GitHub projects.

This project was completed as part of my data analytics learning journey, combining business understanding with technical tools to simulate a real-world analytics workflow.
