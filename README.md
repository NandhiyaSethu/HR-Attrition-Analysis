# HR Attrition Analysis
### Identifying Employee Attrition Patterns Using Google Sheets and Tableau Public

---

## Project Overview

This project analyses **IBM HR employee data** to identify which employee segments are most at risk of leaving the company. The goal was to answer a core business question:

> *"Who is leaving, why are they leaving, and what can the company do to retain them?"*

Employee attrition costs companies **6–9 months of salary** per departed employee. Understanding the root causes enables HR teams to take targeted action before employees resign.

---

## Live Dashboard

🔗 **[View Dashboard on Tableau Public →](https://public.tableau.com/app/profile/nandhiya.s/viz/HRAttrition_17774538480190/Dashboard2)**

---

## Tools and Technologies

| Tool | Purpose |
|---|---|
| **Google Sheets** | Data exploration, validation, pivot tables |
| **Tableau Public** | Interactive dashboard and visualisation |
| **GitHub** | Version control and portfolio hosting |

---

## Dataset

| Detail | Info |
|---|---|
| Source | IBM HR Analytics Employee Attrition Dataset — Kaggle |
| Rows | 1,470 employees |
| Columns | 35 features |
| Target variable | Attrition (Yes/No) |

### Key Columns Used

| Column | Description |
|---|---|
| Attrition | Whether employee left (Yes/No) |
| Department | Sales / R&D / Human Resources |
| Age | Employee age |
| OverTime | Whether employee works overtime (Yes/No) |
| JobSatisfaction | Satisfaction score 1–4 |
| MonthlyIncome | Monthly salary |
| YearsAtCompany | Tenure in years |

---

## Problem Statement

The company has an overall attrition rate of **16.1%** — meaning 237 out of 1,470 employees have left. This analysis identifies which departments, age groups, and working conditions drive the highest attrition, and provides recommendations to reduce it.

---

## Key Findings

### 1. Sales Department Highest Risk
- Sales department attrition rate: **21%** — highest of all departments
- R&D department is most stable at **14%**
- Human Resources attrition: **19%**
- **Recommendation:** Review sales incentive structure, quota pressure, and work-life balance in the Sales team

### 2. Young Employees Leave Most
- Employees **Under 25** leave at **39.2%** — more than double the company average
- Attrition drops significantly after age 35
- Age group breakdown:

| Age Group | Attrition Rate |
|---|---|
| Under 25 | 39.2% |
| 25–34 | 20.2% |
| 35–44 | 10.1% |
| 45+ | 11.5% |

- **Recommendation:** Introduce structured mentorship and clear career progression plans for employees in their first 2 years

### 3. Overtime is the Strongest Predictor
- Employees working overtime leave at **30.5%**
- Non-overtime employees leave at only **10.4%**
- This is a **3x attrition multiplier** from a single factor
- **Recommendation:** Conduct immediate workload audit for overtime-heavy teams. Redistribute work to reduce sustained overtime.

---

## Dashboard

The Tableau Public dashboard contains:

| Visual | Insight shown |
|---|---|
| KPI Cards | Total Employees · Attrited · Attrition Rate |
| Bar Chart — Department | Which department loses the most people |
| Bar Chart — Age Group | Which age group is most at risk |
| Bar Chart — Overtime | How overtime multiplies attrition risk |

🔗 **[View Live Dashboard →](https://public.tableau.com/app/profile/nandhiya.s/viz/HRAttrition_17774538480190/Dashboard2)**

---

## Data Preparation in Google Sheets

Before loading into Tableau the following steps were done in Google Sheets:

| Step | Action |
|---|---|
| Import | Loaded IBM HR CSV — 1,470 rows · 35 columns |
| Validation | Verified 237 attritions (16.1% rate) using COUNTIF |
| Calculated column | Added AttritionNum (Yes=1, No=0) for numeric calculations |
| Calculated column | Added AgeGroup (Under 25 / 25–34 / 35–44 / 45+) |
| Pivot 1 | Attrition by Department |
| Pivot 2 | Attrition by OverTime |
| Pivot 3 | Attrition by Age Group |
| Cross-check | Verified all pivot totals match (237 attrited / 1470 total) |

---

## Key Metrics

| Metric | Value |
|---|---|
| Total Employees | 1,470 |
| Employees Attrited | 237 |
| Overall Attrition Rate | 16.1% |
| Highest Risk Department | Sales — 21% |
| Lowest Risk Department | R&D — 14% |
| Highest Risk Age Group | Under 25 — 39.2% |
| Overtime Attrition Rate | 30.5% |
| Non-Overtime Attrition Rate | 10.4% |
| Overtime Attrition Multiplier | 3x |

---

## Business Recommendations

1. **Conduct workload audit for overtime teams** — overtime is the single strongest predictor of attrition at 3x the rate
2. **Create mentorship programme for under-25 employees** — 39.2% attrition in this group is unsustainable and costly
3. **Review Sales department compensation** — 21% attrition suggests quota pressure or pay dissatisfaction
4. **Monitor job satisfaction scores quarterly** — use as an early warning indicator before attrition happens

---

## Repository Structure

```
hr-attrition-analysis/
├── README.md
├── data/
│   └── HR_Attrition_Clean.csv
└── insights/
    └── key_findings.md
```

---

## Google Sheets Workbook

🔗 **[View Data Preparation Workbook →]https://docs.google.com/spreadsheets/d/1FKdZYegAthOKwVugPKyStaioRGtTlXp55Y0eBXcQNGM/edit?gid=1232206422#gid=1232206422**

Contains:
- Raw Data tab — original IBM dataset
- Analysis tab — with AttritionNum and AgeGroup columns
- Pivot1-Dept — attrition by department
- Pivot2-OverTime — attrition by overtime
- Pivot3-AgeGroup — attrition by age group
- Summary — key findings and recommendations

---

## About Me

This project demonstrates data preparation, pivot table analysis, and dashboard storytelling skills.

- LinkedIn: [your LinkedIn URL]
- GitHub Portfolio: [your GitHub URL]
- E-commerce Analysis Project: [link to Project 3 repo]
- Email: nandhiyadevi2000@gmail.com

---
