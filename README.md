# Loan and Credit Risk Analysis

## Table of Contents
- [Problem Statement](#Problem-Statement)
- [Project Scope](#Project-Scope)
- [Out of Scope](#Out-of-Scope)
- [Objectives](#Objectives)
- [Dashboard Tabs](#Dashboard-Tabs)
- [Data Source](#Data-Source)
- [Tools](#Tools)
- [Data cleaning and preperation](#Data-cleaning-and-preperation)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Audiences / Stakeholders Mapping](#Audiences-/-Stakeholders-Mapping)

### Problem Statement
The organization faces increasing fraud risk and credit exposure, which can lead to financial losses, regulatory challenges, and reputational damage. Currently, there is a lack of consolidated, actionable insights that allow executives, risk managers, and operational teams to monitor suspicious activities, understand the underlying causes of fraud, and evaluate credit risk effectively.

### Project Scope
• Reduce fraud risk by providing actionable insights through dashboards.
• Highlight suspicious activities and anomalies in transactions and customer behavior.
• Uncover underlying causes of fraud to inform mitigation strategies.
• Support the development of effective monitoring strategies for existing and emerging risks.
• Provide descriptive and diagnostic analytics on credit risk, fraud, and customer behavior.
### Out of Scope
• Predictive analytics or insights derived from advanced machine learning models.
• AI-based risk forecasting or automated recommendation engines.
• Analysis beyond historical and current trends in fraud, credit risk, and customer behavior.

### Objectives
#### Executive Summary Dashboard
• Provide executives with a high-level view of fraud risk and credit exposure.
• Enable data-driven strategic decision-making by consolidating key financial, credit, and fraud indicators.
• Improve organizational transparency and accountability by offering a single source of truth for stakeholders.
#### Credit Analysis Dashboard
• Assess borrower risk profiles through metrics such as debt-to-income ratio, late payment frequency, and account status.
• Identify early warning signals of potential defaults or credit deterioration.
• Support credit officers and risk managers in making informed lending decisions and reducing non-performing loans.
• Provide regulatory-compliant insights into credit portfolio health.
#### Fraud Detection Dashboard
• Detect suspicious activities and anomalies through advanced fraud metrics and behavioral patterns.
• Analyze underlying causes of fraud to strengthen risk controls.
• Support fraud analysts and compliance officers in prioritizing investigations and mitigating losses.
• Enable proactive fraud prevention strategies by identifying high-risk accounts, behaviors, and transactions.
• Enhance regulatory reporting and governance by maintaining audit-ready fraud insights.

### Dashboard Tabs
• Executive Summary
• Credit Risk Analysis
• Fraud Detection Analysis
• Customer Overview

### Data Sources
- Customer records (CSV) format
- Transaction history (CSV) format
- Credit bureau data (CSV) format
- Loan application (CSV) format
- Credit scores (CSV) format
- Fraud indicators (CSV) format
- Risk labels (CSV) format
- Branch information (CSV) format
- Fraud Transactions (CSV) format

### Tools
- Excel for data validation
- SQL for data analysis and testing data consitency and accuracy
- Power Query for data preperation for loading
- Power BI Desktop data modeling, developing dashboards.
- Power BI Service creating Worksapce for collaboration and configuring the security and permision level.
- Power BI App published dashboards.

### Data cleaning and preperation
1- Before touching the data, I first:
- Reviewed all tables (customers, loans, transactions, fraud, credit scores).
- Identified grain (customer-level, loan-level, transaction-level).
- Mapped how tables should connect (Customer → Loan → Transaction).
- Defined what metrics the business needed (risk, fraud, portfolio KPIs).
2- After loading the data into Power BI / SQL:
- Checked column types (dates, currency, percentages, IDs).
- Scanned for:
 - Nulls and blanks
 - Duplicate IDs
- Outliers (negative amounts, impossible ages, zero credit scores)
- Compared row counts across tables to detect missing joins.
3- I cleaned and standardized the data:
- Removed duplicate customers, loans, and transactions.
- Handled missing values:
 - Filled or flagged null credit scores
 - Removed unusable records
 - Created “Unknown” categories where needed
- Standardized formats:
 - Unified date formats
 - Normalized region names (e.g., “Vancouver BC” → “Vancouver”)
 - Cleaned profession titles (e.g., “Software Dev”, “SWE” → “Software Developer”)
- Converted currencies and numeric fields to consistent units.
4- I defined Business Logic Layer)
- created new fields such as:
 - Age groups (Under 25, 25–34, 35–45, 45+)
 - Credit tiers (Prime, Near Prime, Subprime, etc.)
 - Customer status (Active vs Inactive)
 - Fraud flags at loan and transaction level
 - High-risk labels based on probability/score thresholds
 - Tenure buckets (New vs Returning customers)
 - Loan categories normalization (Emergency, Auto, Personal, etc.)

### Exploratory Data Analysis
EDA Involved exploring the key question such as:

- How healthy is our loan portfolio, where are our biggest credit and fraud risks, and what actions should the business take to reduce exposure and improve decision-making?
- Are we growing safely or creating future losses?
- Who are our customers and which segments are risky?
- Which branches does show the higher  risk of fraud loan?
- Where is the bank most financially exposed, and why?
- Where is fraud happening, how fast is it growing, and where should we intervene?
- 
### Audiences / Stakeholders Mapping
• Top-Level: Executives, Board, Investors
• Mid-Level: Credit risk managers, compliance officers, fraud analysts, finance team
• Operational-Level: Loan officers, IT/security teams, operations managers
#### Stakeholder Influence Level Interest Level

|Stakeholder|Influence Level|Interest Level|
|-----------|---------------|--------------|
|Executives Board|High|High|
|Credit Risk Managers|High|High|
|Fraud Analysts|Medium-High|High|
|Compliance Officers|Medium-High|High|
|Finance Team|Medium|Medium-High|
|Loan Officers|Medium|Medium|
|IT / Security Teams|Medium|Medium|

### Purpose of Each Tab
• Executive Summary: Consolidates high-level organizational performance, highlighting credit portfolio health, fraud exposure, and financial risk for strategic decision-making.
• Credit Risk: Ensures financial stability by evaluating borrower risk, minimizing potential losses, and supporting regulatory compliance.
• Fraud Detection Analysis: Facilitates early detection of fraud, reduces financial and reputational losses, and strengthens governance.
• Customer Overview: Displays detailed profiles and payment behavior, using sample cases to uncover underlying issues affecting trust and repayment.

### Design and Visualization
• Include 7–10 key measurements per dashboard.
• Visuals: Bar charts, line graphs, trend analysis, and drill-down capabilities.
• Include brand logo or image link at the top of each tab.

### Fraud Prevention Checks
1. Scan applicants against Deceased ID database to prevent identity fraud.
2. Detect potential fraud by spotting irregularities or misuse in names, addresses, SINs, and telephone numbers.
3. Identify duplicated accounts.

### Appendix: Interview / Requirements Questions
• Stakeholders and usage
• KPIs and visualization preferences
• Frequency and refresh requirements
• Drill-down and filtering needs
• Business rules and constraints




