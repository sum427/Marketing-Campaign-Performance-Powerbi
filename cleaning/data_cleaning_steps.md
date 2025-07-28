Data Cleaning Steps – Marketing Campaign Dataset
This document outlines the full set of actions taken to clean and prepare the dataset prior to analysis and visualisation in Power BI.

1. Initial Data Load and Review
Imported the raw marketing campaign data into Excel.

Reviewed the dataset for column consistency, missing values, formatting errors and general structure.

2. Column Splitting and Standardisation
Split the original Target_Audience column into two new columns for clarity:

Target_Age_Range (e.g., “18–24”, “25–34”)

Target_Gender (e.g., “Male”, “Female”, “All”)

Renamed the Duration column to Duration_Days.

Removed the text "days" from values like "30 days", "60 days", etc., leaving only numeric values.

3. Data Formatting and Cleanup
Removed duplicates to ensure accurate aggregation and analysis.

Trimmed leading and trailing spaces in all text fields.

Standardised capitalisation (e.g., “Facebook” not “facebook”).

Ensured all date columns were in proper date format (YYYY-MM-DD).

Removed currency symbols ($) from the Acquisition_Cost column and converted values to numeric format.

4. Created New Calculated Columns
The following metrics were derived for deeper analysis:

Duration_Weeks
→ Converted Duration_Days into weeks (rounded to 1 decimal place):
Duration_Weeks = Duration_Days / 7

CTR (Click Through Rate)
→ Measures ad effectiveness:
CTR = (Clicks / Impressions) × 100

CPC (Cost Per Click)
→ Evaluates ad efficiency:
CPC = Spend / Clicks

Engagement_Rate
→ Captures total user interaction:
Engagement Rate = (Engagements / Impressions) × 100

5. FinaliSation
Verified data integrity and consistency across all rows and columns.

Saved the cleaned dataset in Excel format (cleaned_marketing_data.xlsx) for use in Power BI.
