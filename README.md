# Amazon-Marketplace-Data
You will analyze Amazon marketplace data for one of our product lines, clean and integrate three CSV files, perform exploratory analysis, build a Power BI dashboard, and recommend ways to cut ad spend without hurting rank. All work must be completed within three hours.
________________________________________
1. Data Cleaning & Integration
 • Open the three CSVs in Google Sheets or Excel. ad_spend_daily.xlxs, keywords_ranking.xlxs, sales_traffic_child_asin.xlxs
 • Fix header typos, convert all dates to MM/DD/YYYY, and standardize every currency value to USD.
 • Remove or flag nulls and duplicates, documenting each action.
 • Perform an outer join on ASIN + Date.
 • Add a Boolean column named _imputed; set it to TRUE if you filled or changed any field in that row.
 Deliverable: analysis_ready.xlsx
  – Sheet 1 Clean_Data (merged table)
  – Sheet 2 README_CLEANING (log with columns: Step #, Action, Reason)
________________________________________
2. Exploratory Analysis
 Create Sheet 3 Summary (in the same workbook). Include:
 a) 90-day totals and daily averages for Sessions, Ordered Sales, and Ad Spend.
 b) The ASIN with the largest organic-rank gain per ad-dollar (show calculation).
 c) A “Data Red Flags” table listing any metric with ≥ 20 % missing values, any negatives, or ≥ 3× spikes; add a ≤ 20-word likely cause for each.
________________________________________
3. Visualisation Challenge
 Import Clean_Data into Power BI Desktop and build ONE dashboard page:
 • Visual A: multi-line chart of keyword ranks (reverse y-axis) for any two keywords; annotate weeks containing imputed data.
 • Visual B: clustered column chart (Total Ad Spend) plus line (Ordered Sales) per ASIN across 90 days.
 • Visual C: treemap or matrix showing Ad Spend by Keyword for the top-spending ASIN.
 • Add slicers for Date range, ASIN, and Keyword.
 Deliverables: assessment.pbix and either a PDF export (dashboard.pdf) or a share link pasted into exec_summary.txt.
________________________________________
4. Gap-Driven Business Insight
 The CFO must cut Ad Spend by 15 % without hurting keyword rank. Using your analysis, propose two data-backed actions (maximum 300 words).
 Place the text in Sheet 4 Recommendations of analysis_ready.xlsx and copy the same text into exec_summary.txt.

Allowed tools: Google Sheets or Excel (including Power Query) and Power BI only. Do not submit Python, R, or SQL scripts. Use US date format (MM/DD/YYYY), treat all currency as USD, and assume the America/Chicago time zone.
