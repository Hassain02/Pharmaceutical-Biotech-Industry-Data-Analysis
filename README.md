# Pharmaceutical-Biotech-Industry-Data-Analysis

 # Overview
This project presents a comprehensive Power BI dashboard analyzing the pharmaceutical and biotechnology industry across multiple dimensions — including biotech funding, clinical trials, disease burden, drug performance, and financial metrics.
It integrates data from several sources and models to uncover insights into investment trends, therapy outcomes, global health impact, and company performance.
<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Overview_Analysis.png"alt="Overview" width="100%">
</p>

<p align="center">
 # Data Model
The data model connects multiple datasets through relational links:

Table	Key Fields	Description
Biotech	acquirer_or_investors, deal_type, value_usd_bn, MegaDeal_flag	Captures biotech funding deals and investor activity.
Clinical_trial	sponsor, therapy_area, duration_months, enrollment_n, estimated_stock_impact_pct	Tracks clinical trial performance and stock impact.
Drugs_data	drug_name, Drug_type, peak_sales_usd_bn_est, sponsor_company	Contains drug approval and sales data.
Diseases	disease, dalys_millions, global_dalys_millions, region	Represents global disease burden metrics.
Pharma_finance	Company_name, revenue_usd_bn, operating_income_usd_bn, pipeline_size_est	Summarizes company financials and R&D spending.
Date_table / Year_table	year, month, quarter	Supports time-based analysis.
tTable	Avg_pipeline, drug_revenue, Profit	Aggregated KPIs for summary visualization.
<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/DataModelling.png"alt="Data Model" width="100%">
</p>

<p align="center">

# Dashboards
1. Clinical Trials Dashboard

<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/clinical_Analsis.png"alt="Clinical Trials Dashboard" width="100%">
</p>

<p align="center">


Total Duration: 17K months

Total Enrollment: 473K participants

Estimated Stock Impact: -575.90%

Oncology leads in trial duration and enrollment.

Novartis shows the highest stock impact (27%), while Sanofi has the lowest (5%).

2. Disease Burden Dashboard

<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Diseases_Analysis%20.png"alt="Disease Burden" width="100%">
</p>

<p align="center">


Total Global DALYs: 360,545M

Top Regions: Africa (8.03K), India (7.19K), China (6.52K)

Leading Diseases: Cardiovascular (17.96%), Neurological (11.99%), Cancer (11.53%)

Lowest Disease Impact: Maternal disorders (1.22%)

3. Biotech Funding Dashboard

<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Investor_details.png"alt=" Biotech Funding" width="100%">
</p>

<p align="center">


Highest Investor: AbbVie

Lowest Investor: Vertex

Largest Deal Type: M&A ($1672.62B)

Most Mega Deals: Roche

Least Mega Deals: Pfizer

4. Pharma Financials Dashboard
<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Pharma_Funding.png"alt="Pharma Financials " width="100%">
</p>

<p align="center">




Total Revenue: $13.98K

Profit Margin: 83.55%

Top Profitable Country: USA (55.69%)

Lowest Profit Country: China (0.28%)

Segment Insights: Big Pharma dominates with $2,373.73B operating income.

5. Drug Performance Dashboard
<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Decomposition%20tree.png"alt="Decomposition tree " width="100%">
</p>

<p align="center">



Top Drug: Pfizer-BioNTech COVID vaccine ($37B revenue)

Lowest Drug: Zoltrer-ride ($0.01B revenue)

Highest Sales Type: Small Molecule ($248.66B Mega Blockbuster)

Lowest Sales Type: Gene Therapy ($8.60B)

# Key Insights Summary
Category	Highlights
Biotech	Roche leads Mega Deals; M&A dominates funding.
Clinical	Oncology trials have longest durations; Infectious therapy shows high Phase 2 stock impact.
Disease	Cardiovascular diseases cause highest DALYs globally.
Drug	Pfizer leads in vaccine revenue; Small Molecule drugs dominate sales.
Pharma	USA shows highest profitability; Big Pharma segment drives majority of income.
<p align="center">
  <img src="https://github.com/Hassain02/Pharmaceutical-Biotech-Industry-Data-Analysis/blob/main/Image/Insights%20.png"alt="Key insights " width="100%">
</p>

<p align="center">

# Data Preparation
Each dataset underwent cleaning and formatting:

Removed blank/null cells.

Standardized text using proper() function.

Added symbols for units (B for Billion, M for Million, $ for currency).

Adjusted columns using conditional logic (ifs() function).

Created flags for MegaDeal (>10B) and RealDeal (≤10B).

# Technologies Used
Tool	Purpose
Power BI	Data modeling, visualization, and dashboard creation
Excel / CSV	Data preprocessing and cleaning
DAX	Calculations and measures
Power Query	Data transformation
Visualization Types	Bar charts, Pie charts, Sankey diagrams, Scatter plots, Line graphs


