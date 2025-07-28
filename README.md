# Marketing Campaign Performance Analysis (Power BI)

This project analyses multichannel marketing campaign performance using **Power BI**. The dataset includes KPIs such as ROI, CTR, conversion rates and user engagement across channels, time and demographics.

## Purpose

To showcase data cleaning, analysis and visualisation skills in a real world business context, focusing on **campaign performance insights** to aid **marketing optimisation**. This project complements my previous SQL case study project: (https://github.com/sum427/Superstore-Sales-Analysis-SQL).

---

## Tools Used

- **Excel**: Data cleaning and preparation
- **Power BI**: Dashboard creation, DAX measures and visual storytelling
- **GitHub**: Version control and portfolio hosting

---
## Repository Structure

cleaning/
Step by step documentation of how the dataset was cleaned and transformed.
Includes:

cleaning_steps.md: Trimming, formatting, column renaming, column splitting (e.g., Target_Audience) and calculated fields (e.g., CTR, CPC, duration_weeks)

dashboard/
Contains the final Power BI dashboard file.
Includes:

marketing_dashboard.pbix: Fully built and interactive dashboard with insights across performance, channels and demographics

data/
Raw and cleaned datasets.
Includes:

marketing_data_raw.xlsx: Original unprocessed dataset

marketing_data_cleaned.xlsx: Cleaned version used for dashboard creation

images/
Screenshots of all Power BI dashboard pages for quick reference.
Includes:

introduction.png, channel_overview.png, monthly_trends.png, demographics.png, conclusion.png, etc.

snippets/
Before and after data transformations and calculated metrics.
Includes:

before_after_columns.md: Sample column values before and after cleaning

calculated_metrics.md: Table showing computed metrics (e.g., average ROI, CTR, conversion rate)

README.md
This file. Contains the project overview, folder breakdown, cleaning explanation and instructions for viewing or reusing the dashboard.
---

## Key Features of the Dashboard

Note: The ROI, CTR and Conversion Rate values used in the dashboard are calculated as averages across channels and time periods. This approach was chosen to simplify comparison, reduce volatility from outliers and present a clearer view of overall performance trends.

###  1. Channel Overview  
- Comparison of average ROI and Average CTR across marketing channels  
- Summary table of channel metrics  
- Key Insights: Identifies most efficient channels, performance variability  

### 2. Monthly Trends  
- Monthly trends of average ROI and CTR  
- Key metrics cards (total clicks, impressions, avg conversion rate)  
- Key Insights: Detects seasonal fluctuations and stable periods

### 3. Channel Performance Over Time  
- Line charts tracking aveverage ROI and CTR monthly by channel  
- Key Insights: Highlights optimisation periods, underperformance flags

### 4. Audience Insights  
- Performance by age group and customer segment (e.g., Foodies, Tech Enthusiasts)  
- Matrix table of average ROI, CTR and conversion rate  
- Key Insights: Reveals top performing demographics for targeting

### 5. Introduction & Conclusion  
- Clear summary of project goals and findings  
- Glossary of marketing KPIs for clarity

---
## Data Cleaning Overview
To prepare the raw dataset for analysis, several cleaning and transformation steps were applied.

### Key Cleaning Steps
Removed duplicates to ensure data integrity

Trimmed whitespaces in categorical fields

Removed dollar symbols from Acquisition_Cost and converted to float

Converted percentages to decimals in Conversion_Rate

Split Target_Audience into two columns: Target_Age_Range and Target_Gender

Standardised the Duration column by removing "days" and renaming it to Duration_Days

The example below highlights only a few affected columns from the original dataset to demonstrate key cleaning steps. The full dataset includes additional fields not shown here.

## Before Cleaning:
| Target_Audience | Duration     | Conversion_Rate  | Acquisition_Cost |
|-----------------|--------------|------------------|------------------|
| Men 18-24       | 30 days      | 4%               | $16174.00        |

## After Cleaning
| Target_Age_Range | Target_Gender | Duration_Days | Conversion_Rate | Acquisition_Cost |
|------------------|---------------|---------------|-----------------|------------------|
| 18-24            | Men           | 30            | 0.04            | 16174            |

## New Metrics Added
| CTR   | CPC  | Engagement_Rate | Duration_Weeks |
|-------|------|-----------------|----------------|
| 26.33%|31.96 | 0.31%           | 4.3            |

See full cleaning process in /cleaning/data_cleaning_steps.md
---

## Glossary (Key Terms)

- **ROI (Return on Investment)**: Profit generated per dollar spent on a channel  
- **CTR (ClicknThrough Rate)**: % of impressions that result in clicks  
- **Conversion Rate**: % of clicks that lead to a successful conversion/action  

---

## Conclusion

This dashboard provides useful insights into multichannel marketing performance. It demonstrates proficiency in cleaning, structuring and visualising data using Power BI, with a focus on **targeted marketing strategies** and **audience segmentation**.  

Ideal for roles in **marketing analytics**, **BI development**, or **data driven strategy**.

---

##  Screenshots

See the [`images/`](./images/) folder for full dashboard views.

---

## Download the Dashboard

You can download and explore the interactive dashboard via the `.pbix` file in the [`dashboard/`](./dashboard/) folder.

---

