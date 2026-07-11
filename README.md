# 📊 HR Analytics Dashboard — Workforce Insights. People Decisions.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Power Query](https://img.shields.io/badge/Power%20Query-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)

> An interactive HR analytics dashboard built in Power BI to uncover employee attrition patterns, workforce demographics, and department-level risk — enabling data-driven people decisions.

---

## 🧾 Project Overview

This dashboard analyses employee attrition across departments, job roles, salary slabs, age groups, and experience levels. It helps HR teams and business leaders identify where talent loss is concentrated, which age groups and salary bands carry the most risk, and how tenure relates to attrition.

**Dataset:** HR Analytics Dataset (`HR_Analytics_Dataset.xlsx`)

---

## 📸 Dashboard Preview

![HR Dashboard](HR%20dashboard.png)

> For the best view, download the `.pbix` file and open it in Power BI Desktop.

---

## 📊 Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Employees | 1,470 |
| Active Employees | 1,229 |
| Attrition Count | 241 |
| Attrition Rate | 16.4% |
| Average Age | 39.5 years |
| Average Experience | 9.68 years |

---

## ✨ Key Features

### 🔢 KPI Cards
- Total Employees, Active Employees, Attrition Count, Attrition Rate %, Average Age, Average Experience
- Instant snapshot of overall workforce health

### 📉 Attrition Analysis
- Attrition by Department — Sales leads with 35% of total attrition, followed by IT and Operations (15% each)
- Attrition by Salary Slab — 0–3 LPA employees show the highest attrition count (88), nearly double the 3–6 LPA band
- JobRole Breakdown matrix — headcount split by job level (1–4) across 8 roles, Manager is the largest role at 405 employees
- Attrition Trend by Experience — attrition peaks sharply at 0 years of experience (24 cases) before tapering off

### 👥 Workforce Demographics
- Age Group Distribution — Active vs Attrition Count across 18–25, 26–35, 36–45, 46–55, and 55+ bands
- Largest workforce segment: 26–35 age group with 408 active employees (33% of active headcount)
- Gender Split: Male 63%, Female 37%

### 🏢 Department-wise Employee Count
- Sales is the largest department by headcount (455 employees), followed by Operations (239) and IT (212)
- Finance (129) and Administration (135) are the smallest departments

### 🎛️ Dynamic Filters
- Department slicer (sidebar)
- Age Group slicer (top bar: 18-25, 26-35, 36-45, 46-55, 55+)

---

## 🛠️ Technical Highlights

### DAX Measures
- Custom Attrition Rate % calculation at overall and department level
- Average Age and Average Experience measures
- Active Employees vs Attrition Count comparison measures for age-group and salary-slab visuals

### Power Query (ETL)
- Data type corrections and null handling
- Salary slab classification (0–3 LPA / 3–6 LPA / 6–10 LPA / 10+ LPA) from raw income data
- Age group binning (18–25, 26–35, 36–45, 46–55, 55+)

### Data Modelling
- Clean single-table model with calculated columns and measures
- Optimised for slicer cross-filtering across all visuals (Department + Age Group)

---

## 🔍 Key Findings

- Sales carries the highest attrition share at 35% of all exits — more than double the next closest department
- Attrition is heavily concentrated in the lowest salary slab (0–3 LPA, 88 cases), suggesting compensation is a key retention lever
- New joiners are the highest flight risk — attrition peaks at 0 years of experience (24 cases) and declines steadily afterward
- The 26–35 age group is both the largest workforce segment (408 active employees) and a major contributor to attrition (80 cases), making it the most critical retention target
- Sales is also the largest department by headcount (455 employees), so its high attrition share compounds into a large absolute talent loss

---

## 📁 Project Structure

```
HR-Dashboard-analysis/
├── HR DASHBOARD ANALYSIS.pbix      # Power BI file
├── HR DASHBOARD ANALYSIS.pdf       # Dashboard PDF preview
├── HR dashboard.png                # Dashboard screenshot
├── HR_Analytics_Dataset.xlsx       # Source dataset
└── README.md
```

---

## 🚀 Getting Started

1. Clone this repository
   ```bash
   git clone https://github.com/ayeshasana0355/HR-Dashboard-analysis.git
   ```
2. Open `HR DASHBOARD ANALYSIS.pbix` in **Power BI Desktop**
3. When prompted, point to `HR_Analytics_Dataset.xlsx` as the data source
4. Click **Refresh** to load the data
5. Use the Department and Age Group filters to explore

---

## 🧰 Tools & Technologies

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard development |
| DAX | Custom measures & attrition calculations |
| Power Query (M) | Data cleaning & feature engineering |
| Excel | Source HR dataset |

---

## 🤝 Connect

If you found this useful or want to discuss the approach, connect on [LinkedIn] (https://www.linkedin.com/in/ayesha-sana-3908a130b?utm_source=share_via&utm_content=profile&utm_medium=member_android)or open an issue.

---

*Built with 💙 using Power BI*
