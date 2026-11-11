# Emergency Room Dashboard

An interactive Power BI dashboard (with a Tableau version of the workbook) analysing emergency room visits: volumes, waiting times, patient mix and satisfaction scores.

## At a glance

| | |
|---|---|
| Visits analysed | 9,216 |
| Period | 1 Apr 2019 to 30 Oct 2020 |
| Average wait time | 35.3 minutes (median 35) |
| Departments referred to | General Practice (1,840), Orthopedics (995), Physiotherapy (276), Cardiology (248), Neurology (193), Gastroenterology (178), Renal (86) |
| Satisfaction score | Recorded for 2,517 of 9,216 visits (about 27%) |

## Dashboard pages (Power BI)

1. **Visit Overview**: donut chart, two line charts, stacked area chart, pivot table, KPI cards and slicers.
2. **Patient Overview**: pie chart, clustered bar chart, two column charts, KPI cards and slicers.
3. **Satisfaction Overview**: line-and-column combo chart, scatter chart, line chart, detail table and slicers.

Pages are linked with navigation buttons.

## Data

`Hospital ER.csv` has one row per visit:

| Column | Meaning |
|---|---|
| `date` | Date and time of the visit |
| `patient_id` | Visit or patient identifier |
| `patient_gender`, `patient_age`, `patient_race` | Demographics |
| `patient_sat_score` | Satisfaction score (blank when not recorded) |
| `patient_waittime` | Wait time in minutes |
| `patient_admin_flag` | Administrative flag from the source data |
| `department_referral` | Department the patient was referred to, or `None` |

## Files

| File | Purpose |
|---|---|
| `EmergencyRoomDashboard.pbix` | Power BI report (open in Power BI Desktop) |
| `ER Health.twbx` | Tableau packaged workbook |
| `Hospital ER.csv` | Source data |

## Tools

Power BI, Tableau.
