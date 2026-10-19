# HR-Analytics-
[README.md](https://github.com/user-attachments/files/33680867/README.md)
# HR Employee Attrition & Retention Dashboard

A Power BI project that analyzes why employees leave a company and which groups are most at risk, so HR can act on the findings.

---

## 1. Business Problem

The company lost **237 of its 1,470 employees (16.12% attrition rate)**. Losing employees is costly (hiring, training, lost knowledge), so HR needs to know:

- Which employee groups leave the most?
- What drives attrition (overtime, pay, tenure, travel, age, marital status)?
- Which departments and job roles are most affected?
- What actions can reduce attrition?

## 2. Objectives

- Clean and prepare the HR employee data.
- Build a data model and the KPIs needed to measure attrition.
- Design an interactive dashboard that lets HR explore the data with slicers and filters.
- Turn the results into clear business insights and recommendations.

## 3. Tools Used

| Stage | Tool |
|---|---|
| Data cleaning & preparation | Power Query (Power BI) |
| Data modeling & measures | Power BI, DAX |
| Dashboard design | Power BI Desktop |
| Documentation & presentation | PDF, PowerPoint |
| Version control | Git & GitHub |

## 4. Dataset

- Source file: `HR_Employee_Attrition_Cleaned`
- 1,470 employees
- Key fields: age group, gender, marital status, department, job role, job level, income, overtime, business travel, tenure, years since last promotion, job satisfaction, stock option level, attrition status.

> TODO: add the data source/link and the number of columns.

## 5. Data Model

| Table | Purpose |
|---|---|
| `Fact_Employee` | One row per employee (demographics, income, tenure, attrition status) |
| `Dim_Job` | Department, job role, job level |
| `Measures_HR` | All DAX measures |
| `Progress Axis` | Helper table used in the dashboard |

Main KPIs: Total Employees, Active Employees, Attrition Rate, Average Monthly Income, Avg Years at Company, Overtime Attrition Rate.

## 6. Dashboard Pages

| Page | What it shows |
|---|---|
| Home | Cover page and navigation |
| Overview | Headline KPIs, attrition by job level, department and age group |
| Drivers | Attrition by tenure, income band, business travel, marital status and overtime |
| Compensation | Income analysis, attrition by job role, stock options and job satisfaction |
| Tenure | Years at company, promotions and number of companies worked |
| Workforce | Headcount by job role, age, education, marital status and gender |
| Insights | Eight key findings, each with a recommended action |

Screenshots are in the [`screenshots/`](screenshots/) folder.

## 7. Key Findings (draft, to be confirmed in Final QA)

- Attrition is highest in the first year (34.9% for 0–1 years vs 8.1% for 10+ years).
- Employees working overtime leave far more (30.5% vs 10.4%).
- Sales Representatives have the highest attrition by role (39.8%).
- Low income is linked to higher attrition (28.6% for under $3K vs 8.9% at $10K+).
- Single employees who work overtime are the highest-risk segment (49.6%).

## 8. Repository Structure

```
HR-Analytics-Project/
├── README.md
├── Final_Submission_Checklist.md
├── dashboard/            # HR_Analytics_Project.pbix
├── documentation/        # Project_Booklet.pdf, Technical_Documentation.pdf
├── presentation/         # HR_Analytics_Presentation.pptx
├── demo/                 # HR_Analytics_Demo.mp4
├── infographic/          # HR_Analytics_Infographic.png
└── screenshots/          # Final dashboard page images
```

## 9. Team

| Member | Role |
|---|---|
| Ahmed Samy | TODO |
| Alzahraa Hassan | TODO |
| Arsany Hany | TODO |
| Sandra Hany | TODO |
| Haneen Tarek | TODO |

## 10. Project Phases and Files

| Phase | Output | Location |
|---|---|---|
| Data understanding & cleaning | Cleaned dataset, Power Query steps | TODO |
| Data modeling & DAX | Data model, measures | `dashboard/` |
| Dashboard design | `.pbix` file | `dashboard/` |
| Testing & final improvements | Final `.pbix` | `dashboard/` |
| Documentation & delivery | Booklet, technical docs, presentation, video, infographic | `documentation/`, `presentation/`, `demo/`, `infographic/` |

## 11. How to View the Project

1. Open `dashboard/HR_Analytics_Project.pbix` in Power BI Desktop.
2. Use the navigation buttons on the left to move between pages.
3. Use the slicers and filters to explore the data.
4. Or watch the demo video in `demo/`.
