# Member Attendance & Fines Analytics

## Project Overview
In student organizations and academic associations, tracking meeting attendance, lateness, and associated fines is frequently handled through manual paper sheets or unstandardized spreadsheets. For this project, I transformed raw attendance logs into a structured, relational dataset, built pivot-based analytical models, and uncovered actionable behavioral and financial insights.    

##  Approach & Methodology
- Data Cleaning & Standardization: Standardized raw attendance inputs using uniform status codes: P (Present), L (Late), E (Excused absence), and U (Unexcused absence).
- Power Query Transformation: Transformed wide-format attendance tables into a clean, normalized long format (one row per member per meeting date) using Power Query (`Unpivot Columns`).
- Multidimensional Analysis: Developed dedicated analytical modules for Attendance, Fines, and Demographics to compute collection rates and fine distributions.
- Statistical Modeling & Outlier Detection: Applied statistical functions (`AVERAGE`, `MEDIAN`, `MODE`, `STDEV.S`) to evaluate distribution shapes and implemented an objective outlier detection rule.
- Chi-Square Contingency Analysis: Performed a Chi-Square test of independence to examine whether unexcused absences are statistically associated with member gender.

## Key Findings
1. Attendance Distribution: The data exhibited a left-skewed distribution where Mean (73%) < Median (80%)} < Mode (91%), indicating strong general engagement with distinct temporal dips on specific dates.
2. Financial Collections: Uncovered a major collection backlog—while 16 members had clean records and 23 settled their dues, 34 members had outstanding balances, including ₦15,600 in unpaid lateness fines and ₦61,500 in unpaid unexcused absence fines.
3. Gender Segmentation & Chi-Square: Female members maintained a higher average attendance rate (77%) compared to males (70%). A Chi-Square test yielded a p-value of 0.0419, confirming a statistically significant dependence between gender and unexcused absences.

## Future Enhancements
- Interactive Dashboarding: Exporting the cleaned model into Power BI or Looker Studio for dynamic date slicers.
- Automated Workflows: Integrating messaging scripts to dispatch automated payment reminders for members exceeding debt thresholds.

---
Created by Okikioluwa Dasho
