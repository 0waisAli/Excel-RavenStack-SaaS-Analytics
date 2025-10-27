# Excel-RavenStack-SaaS-Analytics-Dashboard
An end-to-end SaaS analytics dashboard built in Excel using Power Query, dynamic KPIs, and interactive simulators to analyze churn, revenue, feature adoption, and customer satisfaction.
📊 RavenStack SaaS Analytics Dashboard (Excel Project)
🧭 Overview

This project demonstrates an end-to-end Excel-based analytics workflow for a fictional SaaS company, RavenStack.
It replicates a real-world business intelligence scenario — combining customer, subscription, feature, churn, and support data into one dynamic, insight-rich Excel dashboard.

Built entirely in Excel + Power Query, this project highlights how a data analyst can use advanced Excel techniques to transform raw business data into meaningful, actionable insights for growth and retention.

🧩 Dataset Description

The dataset represents the core elements of a SaaS company’s business model and includes 5 interlinked data tables:

Sheet	Description
ravenstack_accounts	Account-level details: company name, country, industry, plan tier, referral source, and signup date.
ravenstack_subscriptions	Subscription data including start/end dates, plan tier, MRR, ARR, churn, upgrades/downgrades, and billing type.
ravenstack_feature_usage	Product usage logs tracking usage count, session durations, beta feature use, and errors per feature.
ravenstack_churn_events	Churn events with reason codes, refund amounts, and whether the account later reactivated.
ravenstack_support_tickets	Customer support tickets with priority, resolution times, satisfaction scores, and escalation flags.

Each dataset was related by a unique account_id or subscription_id, allowing for complete business analysis from signup → usage → churn → support.

⚙️ Data Cleaning & Transformation (Power Query)

All five tables were loaded and processed in Power Query, resulting in a single master dataset: MergedTable.

Key data engineering steps:

Standardization

Cleaned column names and formats.

Converted date fields into valid date types.

Normalized TRUE/FALSE values → 1/0.

Derived Columns

SignupMonth, SignupYear for time-based analysis.

ARR_Calculated = MRR × 12 for monthly subscriptions.

ActiveSubscriptionFlag to isolate active customers.

Aggregations

Feature Usage: Total usage count, total duration, total errors, beta usage count.

Support Tickets: Total tickets, average resolution time, average satisfaction score, escalations count.

Merging

Merged all tables on account_id and subscription_id via left joins.

Final dataset contained metrics from across the SaaS lifecycle.

📈 Dashboard Components

The dashboard (on the Dashboard sheet) is designed for business decision-makers to quickly assess company health and performance.
It contains four main sections:

1️⃣ Key Metrics (KPI Cards)

Instant overview of business performance:

Total Accounts

Active Subscriptions

Average MRR / ARR

Churn Rate (%)

Reactivation Rate (%)

Average Satisfaction Score

Beta Feature Adoption Rate (%)

Total Support Tickets

Each KPI is dynamically calculated from the merged dataset, automatically updating with filtered inputs.

2️⃣ Churn & Retention

Visualization: Column chart — Churn Reason vs Signup Month/Year
KPIs: Reactivation Rate, Total Refunds

💡 Insight: Identify why customers leave, track churn trends over time, and measure success of win-back efforts.

3️⃣ Feature Usage & Beta Adoption

Visualization: Bar/Column Chart by Plan Tier

Total Usage Count

Beta Feature Adoption %

💡 Insight: Understand how usage varies by plan tier and which users engage with beta or experimental features.

4️⃣ Support & Customer Experience

Visualizations:

Avg. Resolution Time by Priority

Customer Satisfaction by Country

💡 Insight: Measure customer experience quality and operational efficiency — key to reducing churn.

5️⃣ 💰 MRR / ARR Simulator (Interactive)

A fully interactive simulator allows users to filter and project revenue based on:

Plan Tier

Billing Frequency

Country

Dynamic metrics update instantly:

Filtered MRR

Filtered ARR

Active Subscriptions / Seats

💡 Insight: Test revenue scenarios under different customer, region, or pricing conditions — just like a business dashboard.

🧠 Skills Demonstrated
Category	Skills
Data Preparation	Power Query (merging, transformations, groupings)
Data Analysis	Excel formulas (SUMIFS, COUNTIFS, IF/AND logic), PivotTables
Visualization	KPI Cards, PivotCharts, Interactive Simulators
Business Metrics	MRR, ARR, Churn, Retention, Feature Adoption, CSAT
Automation	Dynamic references and slicer integration
💼 Use Case

This project mirrors what a Data Analyst or Business Intelligence Associate would create for a SaaS startup or growth team:

Monitor revenue and subscription metrics

Identify customer churn causes

Analyze feature adoption

Measure support efficiency

It demonstrates not just Excel mastery, but also business acumen — turning data into insights that drive retention and growth.

🚀 How to Use

Open RavenStack_SaaS_Analytics.xlsx

Explore the raw dataset under the MergedTable sheet

View the Dashboard sheet for analytics visualizations

Use dropdown filters (Plan Tier, Billing, Country) to simulate revenue outcomes

📚 Author

Owais Ali
🎓 BSc Computer Science (CGPA 3.6)
📍 Lahore, Pakistan
📧 work.owaisaly@gmail.com

🔗 LinkedIn
 | GitHub
