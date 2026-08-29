# 📊 Employee Attrition Analysis Dashboard

An end-to-end **Employee Attrition Analysis** project built using **Microsoft Excel and Power BI**. This project analyzes employee turnover patterns and identifies key factors associated with employee attrition.

---

## 📌 Project Overview

Employee attrition is an important HR challenge that can affect productivity, hiring costs, employee morale, and organizational performance.

This project uses employee data to analyze attrition across different dimensions such as:

* Department
* Job Role
* Overtime
* Years at Company
* Job Satisfaction
* Monthly Income
* Performance Rating

The analysis transforms raw employee data into interactive dashboards and actionable HR insights.

---

## 🎯 Objectives

* Calculate key employee attrition KPIs.
* Identify departments with higher attrition.
* Analyze attrition across different job roles.
* Understand the relationship between overtime and attrition.
* Analyze attrition based on employee tenure.
* Examine the relationship between job satisfaction and attrition.
* Explore monthly income and performance rating patterns.
* Build an interactive Power BI dashboard.
* Provide data-driven insights to support employee retention strategies.

---

## 🛠️ Tools & Technologies

| Tool                   | Purpose                                              |
| ---------------------- | ---------------------------------------------------- |
| **Microsoft Excel**    | Data analysis, PivotTables, charts and KPI dashboard |
| **Power BI**           | Interactive dashboard and data visualization         |
| **DAX**                | KPI and attrition-rate calculations                  |
| **Data Visualization** | Presenting HR trends and insights                    |

---

## 📂 Dataset

The dataset contains **1,470 employee records** and includes **35 attributes** related to employee demographics, job information, compensation, satisfaction, performance, and employment history.

### Important Columns

* `EmployeeNumber`
* `Age`
* `Attrition`
* `Department`
* `JobRole`
* `MonthlyIncome`
* `JobSatisfaction`
* `OverTime`
* `PerformanceRating`
* `YearsAtCompany`
* `YearsInCurrentRole`
* `YearsSinceLastPromotion`
* `YearsWithCurrManager`

---

## 📈 Key Performance Indicators

| KPI                    |      Value |
| ---------------------- | ---------: |
| Total Employees        |  **1,470** |
| Employees Left         |    **237** |
| Employees Stayed       |  **1,233** |
| Overall Attrition Rate | **16.12%** |

---

## 📊 Excel Analysis

The Excel analysis includes:

1. **KPI Summary**
2. **Attrition by Overtime**
3. **Attrition by Job Role**
4. **Attrition by Tenure**
5. **Job Satisfaction Analysis**
6. **Monthly Income Analysis**
7. **Performance Rating Analysis**
8. **Final Employee Attrition Dashboard**

PivotTables and charts were used to summarize employee attrition patterns.

---

## 📊 Power BI Dashboard

The Power BI dashboard provides an interactive view of employee attrition.

### Dashboard Components

* Total Employees KPI
* Employees Left KPI
* Employees Stayed KPI
* Attrition Rate KPI
* Attrition by Department
* Attrition by Overtime
* Attrition by Job Role
* Attrition by Years at Company
* Attrition by Job Satisfaction
* Attrition by Monthly Income
* Attrition by Performance Rating

### Interactive Filters

Users can filter the dashboard using:

* **Department**
* **Job Role**
* **Overtime**

These slicers allow users to explore employee attrition patterns interactively.

---

## 🧮 DAX Measures

### Total Employees

```DAX
Total Employees =
COUNTROWS('Employee Data')
```

### Employees Left

```DAX
Employees Left =
CALCULATE(
    COUNTROWS('Employee Data'),
    'Employee Data'[Attrition] = "Yes"
)
```

### Employees Stayed

```DAX
Employees Stayed =
CALCULATE(
    COUNTROWS('Employee Data'),
    'Employee Data'[Attrition] = "No"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Employees Left],
    [Total Employees],
    0
)
```

---

## 🔍 Key Business Questions

This project aims to answer questions such as:

* What is the overall employee attrition rate?
* Which departments experience higher attrition?
* Which job roles have greater employee turnover?
* Does overtime appear to be associated with higher attrition?
* Which tenure groups have higher attrition?
* Does job satisfaction relate to employee turnover?
* How does monthly income vary across employees who leave and stay?
* Is there a noticeable relationship between performance rating and attrition?

---

## 💡 Business Insights

The dashboard can help HR teams identify employee groups that may require additional attention.

Potential areas for retention strategies include:

* Managing excessive overtime and workload.
* Improving employee engagement and job satisfaction.
* Monitoring high-attrition departments and job roles.
* Strengthening onboarding and early-career support.
* Reviewing compensation and career-growth opportunities.
* Developing targeted employee retention programs.

> **Note:** Final business conclusions should be based on the calculated attrition rates and patterns observed in the dashboard rather than assumptions.

---

## 📁 Project Structure

```text
Employee-Attrition-Analysis/
│
├── data/
│   └── employee_data.xlsx
│
├── excel/
│   └── employee_attrition_analysis.xlsx
│
├── powerbi/
│   └── employee_attrition_dashboard.pbix
│
├── screenshots/
│   ├── excel_dashboard.png
│   └── powerbi_dashboard.png
│
└── README.md
```

---

## 🚀 How to Use

### Excel

1. Open the Excel workbook.
2. Review the KPI Summary.
3. Explore the PivotTables and charts.
4. Use the dashboard for employee attrition analysis.

### Power BI

1. Open the `.pbix` file using Power BI Desktop.
2. Review the KPI cards and visualizations.
3. Use the slicers to filter by Department, Job Role, and Overtime.
4. Explore the dashboard to identify attrition patterns.

---

## 📌 Project Outcome

This project demonstrates how **Excel and Power BI can be used together for HR analytics**, transforming employee-level data into KPIs, visualizations, and actionable business insights.

The dashboard provides HR stakeholders with a simple way to explore employee attrition and identify areas where retention efforts may be required.

---

## 👤 Author

**Your Name**

*Data Analytics | Excel | Power BI | HR Analytics*

---

⭐ If you find this project useful, feel free to star the repository.
