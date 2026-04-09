🌍 World Bank ITS – Digital Readiness Dashboard

ET Consultant Technical Assessment Project

📌 Overview

This project is based on a technical assessment inspired by the World Bank Group ITS (Information & Technology Solutions) Transformation Data Insights team.

The objective was to analyze digital readiness and IT performance across countries, and deliver a data-driven dashboard to support leadership decision-making.

The entire workflow simulates a real-world analytics task:
➡️ Data cleaning → Data modeling → Visualization → Business insights

🎯 Problem Statement

Leadership needs a quick way to understand:

How digital readiness varies across countries
How IT project performance differs across regions
Which countries/regions need priority investment

The goal was to build a clear, executive-level dashboard using limited time (90 minutes).

📂 Dataset
File: WB_ICT_Development_Dataset.csv
Records: 150 rows
Coverage: 25 countries, 2018–2023
Key Features:
🌐 Internet usage (% of population)
📱 Mobile subscriptions per 100 people
💰 GDP per capita (USD)
🧠 Digital workforce skills (%)
🏗️ IT project completion rate (%)
🔐 Cybersecurity readiness score (0–100)

⚠️ ~5% of the dataset contains missing values (handled during preprocessing).

🛠️ Tools & Technologies
Microsoft Excel → Data analysis & validation
Power BI Desktop → Dashboard & visualization
DAX → Calculations & KPIs
Power Query → Data cleaning & transformation
📊 Project Structure
🔹 Part A – Excel Analysis

Performed initial data validation and aggregation:

Used AVERAGEIFS to compute Internet usage by income group (2023)
Built a Data Quality Report:
Missing Count
Missing %
Risk Classification:
✅ Clean (<3%)
⚠️ Review (3–10%)
❗ High Risk (>10%)
Created a Pivot Table:
IT Project Completion Rate by Region & Year
Applied conditional formatting (performance comparison)
🔹 Part B – Power BI Dashboard
📄 Page 1 – Executive Overview

✔️ Data Modeling

Ensured correct data types in Power Query
Created calculated column:
Digital_Readiness_Score = 
(0.4 * [Internet_Users_Pct]) +
(0.35 * [Digital_Skills_Workforce_Pct]) +
(0.25 * [Cybersecurity_Index_Score])

✔️ KPIs (Dynamic with Year Slicer)

Avg Internet Users %
Avg Digital Readiness Score
Avg IT Project Completion Rate

✔️ Time Intelligence

YoY Internet Change = 
[Internet Users %] - CALCULATE([Internet Users %], PREVIOUSYEAR('Table'[Year]))
Conditional formatting:
🟢 Positive growth
🔴 Negative growth

✔️ Geo Visualization

World map showing:
Internet usage by country
Colored by Income Group
📈 Key Insights
📉 Regions with low digital skills often also show lower IT project success rates
🌍 Higher-income countries generally have higher digital readiness scores
📊 Internet adoption is increasing YoY, but growth is uneven across regions
⚠️ Some regions show strong infrastructure but weak workforce readiness
🧠 Business Recommendation

Based on the analysis:

👉 Regions with low digital skills but moderate internet penetration should be prioritized

These regions already have infrastructure
Investment in workforce skills will deliver faster ROI
🧹 Data Quality Handling
Identified missing values using:
Excel (COUNTBLANK)
Power BI profiling
Handling approach:
Used imputation (averages/region-based) where appropriate
Flagged critical gaps for transparency

📌 Impact:

Minimal impact (~5% missing)
Dashboard remains reliable for directional insights
🚀 How to Use
Open .pbix file in Power BI Desktop
Use the Year slicer to explore trends
Interact with:
KPI cards
Map visual
Trend insights
📌 Files Included
WB_ICT_Development_Dataset.csv → Raw dataset
Dashboard.pbix → Power BI dashboard
Answers.docx → Written analysis
README.md → Project documentation
💡 What This Project Demonstrates
End-to-end data analytics workflow
Strong Power BI & DAX skills
Ability to translate data into business insights
Handling real-world data quality issues
Building executive-ready dashboards

📬 About Me

I’m a Data Analyst with experience in:

SQL, Python, Power BI
ETL pipelines (AWS Glue, Snowflake)
Data modeling & dashboarding

📌 This project reflects my ability to deliver impactful insights under time constraints.
