# Tableau-Project
# 📊 HR Analytics Dashboard — Employee Attrition Analysis

![Tableau](https://img.shields.io/badge/Tableau-Desktop-blue?logo=tableau)
![Dataset](https://img.shields.io/badge/Dataset-IBM%20HR%20Analytics-orange)
![Records](https://img.shields.io/badge/Records-1%2C470%20Employees-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

This project presents an interactive **HR Analytics Dashboard** built using **Tableau**, designed to help HR professionals and business leaders analyze employee attrition patterns within an organization.

By visualizing key HR metrics such as attrition rate, department-wise distribution, job satisfaction, income trends, and demographic breakdowns, this dashboard enables data-driven decisions to improve employee retention, optimize workforce planning, and reduce turnover costs.

The analysis is based on the IBM HR Analytics Employee Attrition & Performance dataset, containing records for **1,470 employees** across **35 features**.

---

## 🎯 Objectives

- Identify the **overall attrition rate** and understand which employee segments are most at risk.
- Analyze attrition across **departments, job roles, age groups, and education fields**.
- Explore the relationship between **salary, job satisfaction, work-life balance**, and employee retention.
- Uncover patterns between **overtime, years at the company**, and attrition likelihood.
- Provide an interactive, executive-ready dashboard for HR stakeholders.

---

## 📁 File Descriptions

| File | Type | Description |
|------|------|-------------|
| `HR_ANALYTICS_DASHBOARD_PROJECT_TAQI.twbx` | Tableau Packaged Workbook | The complete Tableau dashboard including all visualizations, calculated fields, and embedded data. Open this file in Tableau Desktop or Tableau Public. |
| `HR-Employee-Attrition.csv` | CSV Dataset | The raw IBM HR Analytics dataset with 1,470 employee records and 35 feature columns used as the data source for the dashboard. |

---

## 🗃️ Dataset Description

| Property | Value |
|----------|-------|
| **Source** | IBM HR Analytics (publicly available) |
| **Rows** | 1,470 employees |
| **Columns** | 35 features |
| **Target Variable** | `Attrition` (Yes / No) |
| **Attrition — Yes** | 237 employees (≈16.1%) |
| **Attrition — No** | 1,233 employees (≈83.9%) |
| **Age Range** | 18 – 60 years (mean: ~37) |
| **Departments** | Research & Development, Sales, Human Resources |

---

## 🔍 Column / Feature Explanation

### 👤 Employee Demographics

| Column | Type | Description |
|--------|------|-------------|
| `Age` | Integer | Employee's current age (18–60) |
| `Gender` | String | Male or Female |
| `MaritalStatus` | String | Single, Married, or Divorced |
| `Over18` | String | Whether the employee is over 18 (all values are "Y") |
| `EducationField` | String | Field of education (Life Sciences, Medical, Marketing, etc.) |
| `Education` | Integer | Education level: 1=Below College, 2=College, 3=Bachelor, 4=Master, 5=Doctor |

### 🏢 Job Information

| Column | Type | Description |
|--------|------|-------------|
| `Department` | String | Department: Research & Development, Sales, Human Resources |
| `JobRole` | String | Job title (Sales Executive, Research Scientist, Manager, etc.) |
| `JobLevel` | Integer | Seniority level (1=Entry to 5=Senior) |
| `BusinessTravel` | String | Frequency of travel: Non-Travel, Travel_Rarely, Travel_Frequently |
| `OverTime` | String | Whether employee works overtime (Yes / No) |
| `StandardHours` | Integer | Standard work hours (80 for all employees) |
| `EmployeeCount` | Integer | Always 1; used for aggregation |
| `EmployeeNumber` | Integer | Unique employee identifier |

### 💰 Compensation & Growth

| Column | Type | Description |
|--------|------|-------------|
| `MonthlyIncome` | Integer | Monthly salary in USD |
| `DailyRate` | Integer | Daily billing or pay rate |
| `HourlyRate` | Integer | Hourly rate of pay |
| `MonthlyRate` | Integer | Monthly rate (different from monthly income) |
| `PercentSalaryHike` | Integer | Percentage increase in salary last year |
| `StockOptionLevel` | Integer | Stock option granted: 0=None to 3=High |

### 😊 Satisfaction & Performance

| Column | Type | Description |
|--------|------|-------------|
| `JobSatisfaction` | Integer | 1=Low, 2=Medium, 3=High, 4=Very High |
| `EnvironmentSatisfaction` | Integer | Satisfaction with work environment (1–4 scale) |
| `RelationshipSatisfaction` | Integer | Satisfaction with workplace relationships (1–4 scale) |
| `WorkLifeBalance` | Integer | 1=Bad, 2=Good, 3=Better, 4=Best |
| `JobInvolvement` | Integer | 1=Low to 4=Very High |
| `PerformanceRating` | Integer | 1=Low to 4=Outstanding |

### 🕒 Tenure & Experience

| Column | Type | Description |
|--------|------|-------------|
| `TotalWorkingYears` | Integer | Total years of work experience |
| `YearsAtCompany` | Integer | Number of years at current company |
| `YearsInCurrentRole` | Integer | Years in the current job role |
| `YearsSinceLastPromotion` | Integer | Years since the last promotion |
| `YearsWithCurrManager` | Integer | Years working under the current manager |
| `NumCompaniesWorked` | Integer | Number of companies worked at previously |
| `TrainingTimesLastYear` | Integer | Number of training sessions attended last year |

### 🎯 Target Variable

| Column | Type | Description |
|--------|------|-------------|
| `Attrition` | String | **Target variable** — whether the employee left: `Yes` or `No` |

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Tableau Desktop / Public** | Dashboard creation, interactive visualizations |
| **Microsoft Excel / CSV** | Raw dataset format and preprocessing |
| **IBM HR Analytics Dataset** | Source data |

---

## ⚙️ Installation Instructions

### Prerequisites

- **Tableau Desktop** (2020.1 or later) — paid license  
  **OR**  
- **Tableau Public** (free) — [Download here](https://public.tableau.com/en-us/s/download)

### Steps

1. **Clone or download this repository:**

   ```bash
   git clone https://github.com/<your-username>/HR-Analytics-Dashboard.git
   cd HR-Analytics-Dashboard
   ```

2. **Open the Tableau workbook:**

   - Launch Tableau Desktop or Tableau Public.
   - Go to **File → Open** and select `HR_ANALYTICS_DASHBOARD_PROJECT_TAQI.twbx`.
   - The `.twbx` file is a packaged workbook — it already includes the dataset, so no separate data connection is needed.

3. *(Optional)* **Explore the raw data:**

   - Open `HR-Employee-Attrition.csv` in Excel, Google Sheets, or any CSV viewer to inspect the data independently.

---

## 📖 Usage Guide

Once the Tableau workbook is open:

1. **Navigate between dashboard sheets** using the tabs at the bottom of the screen.
2. **Use filters** (e.g., Department, Gender, Job Role) on the right-hand panel to slice the data interactively.
3. **Hover over charts** to see detailed tooltips with exact values.
4. **Click on any visual element** (bar, pie slice, etc.) to cross-filter other charts on the same dashboard.
5. **Export visuals** via **Worksheet → Export → Image** or use **Dashboard → Export as PDF** for reporting.

---

## 🧹 Data Preprocessing Steps

The following preprocessing considerations apply to the raw CSV before or during Tableau analysis:

1. **Removed constant columns:** `EmployeeCount`, `StandardHours`, and `Over18` have zero variance (all values identical) and do not contribute to analysis — filtered out in Tableau views.

2. **Encoded target variable:** `Attrition` is a binary string (`Yes`/`No`). A calculated field in Tableau converts this to a numeric `[Attrition Flag]` (1/0) for rate calculations.

3. **Ordinal interpretation:** Satisfaction and rating columns (e.g., `JobSatisfaction`, `WorkLifeBalance`) are treated as ordered categorical variables with labeled aliases (1=Low, 2=Medium, 3=High, 4=Very High).

4. **Binning age groups:** Age is grouped into bins (18–25, 26–35, 36–45, 46–55, 56–60) using Tableau's built-in bin/group feature for demographic breakdowns.

5. **No missing values:** The IBM dataset is clean with no null entries, so no imputation was required.

---

## 📊 Example Outputs / Key Insights

| Insight | Finding |
|---------|---------|
| **Overall Attrition Rate** | ~16.1% of employees left (237 out of 1,470) |
| **Highest Attrition by Department** | Sales has a disproportionately high attrition share |
| **Most Affected Job Role** | Sales Representatives and Laboratory Technicians |
| **Overtime Impact** | Employees working overtime show significantly higher attrition |
| **Income & Attrition** | Employees who left tend to have lower monthly incomes |
| **Work-Life Balance** | Poor work-life balance (rating = 1) correlates with higher turnover |
| **Age Group** | Younger employees (18–30) exhibit higher attrition rates |
| **Years at Company** | Highest risk in the first 1–3 years of employment |

> 💡 **The dashboard surfaces these findings interactively**, allowing HR teams to drill down by any combination of filters.

---

## 🗂️ Folder Structure

```
HR-Analytics-Dashboard/
│
├── HR_ANALYTICS_DASHBOARD_PROJECT_TAQI.twbx   # Tableau packaged workbook (dashboard + data)
├── HR-Employee-Attrition.csv                  # Raw dataset (1,470 rows × 35 columns)
└── README.md                                  # Project documentation (this file)
```

---

## 🚀 Future Improvements

- [ ] **Predictive Modeling:** Integrate a Python/R-based logistic regression or random forest model to predict individual attrition probability.
- [ ] **Python EDA Notebook:** Add a Jupyter Notebook with exploratory data analysis, correlation heatmaps, and feature importance plots.
- [ ] **Tableau Server / Public Publishing:** Publish the dashboard to Tableau Public for browser-based, shareable access.
- [ ] **Time-Series Analysis:** Incorporate hire dates to analyze attrition trends over time.
- [ ] **Department-Specific Sub-Dashboards:** Build drill-through dashboards per department for targeted HR use.
- [ ] **Benchmarking:** Compare internal attrition rates against industry benchmarks.
- [ ] **HR Recommendations Panel:** Add an automated insight panel using Tableau's Ask Data / Explain Data features.

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

The dataset (`HR-Employee-Attrition.csv`) is sourced from the publicly available **IBM HR Analytics dataset** on Kaggle and is used here for educational and portfolio purposes only.

---

## 👤 Author

**mOHAMMED Taqi**


---

> ⭐ If you found this project helpful, please consider giving it a **star** on GitHub!
