
 # 🏥 Healthcare Patient Analytics: End-to-End Data Analysis & Interactive Dashboard

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-lightblue) ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange) ![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-teal) ![Excel](https://img.shields.io/badge/Microsoft%20Excel-Dashboard-green?logo=microsoft-excel)

---

## 📌 Project Overview

This end-to-end data analytics project explores a **55,500-row healthcare dataset** containing patient admissions, billing, diagnoses, and test results. The project covers the full data analyst workflow — from raw data cleaning to exploratory analysis, Python visualizations, and a polished Excel KPI dashboard.

This project was built as a **portfolio project** to demonstrate real-world data analyst skills including data wrangling, EDA, storytelling with data, and business dashboard design.

---

## 🎯 Objectives

- Clean and prepare raw healthcare data for analysis
- Perform exploratory data analysis (EDA) to uncover trends and patterns
- Visualize key insights across billing, admissions, and patient outcomes
- Build an interactive Excel dashboard with KPIs, Pivot Tables, and Slicers

---

## 🗂️ Dataset

| Feature | Detail |
|---|---|
| Source | Synthetic Healthcare Dataset |
| Rows | 55,500 |
| Columns | 15 |
| Format | CSV |

**Key Columns:** Name, Age, Gender, Blood Type, Medical Condition, Date of Admission, Doctor, Hospital, Insurance Provider, Billing Amount, Room Number, Admission Type, Discharge Date, Medication, Test Results

---

## 🛠️ Tools & Technologies

- **Python** — Pandas, Matplotlib, Seaborn, NumPy
- **Microsoft Excel** — Pivot Tables, Slicers, Conditional Formatting, Charts
- **Jupyter Notebook** — Analysis & Visualization

---

## 🔄 Project Workflow

### 1. 🧹 Data Cleaning (Python)
- Standardized inconsistent name casing using `.str.title()`
- Converted date columns to proper `datetime` format
- Removed negative Billing Amount values
- Engineered new features:
  - **Length of Stay** = Discharge Date − Admission Date
  - **Age Group** (binned: 10–90 in 10-year intervals)
  - **Admission Year** and **Admission Month**
- Final cleaned dataset: **55,447 rows**

### 2. 📊 Exploratory Data Analysis (Python)
- Univariate analysis: Age, Billing Amount, categorical distributions
- Bivariate analysis: Billing by condition, Length of Stay by admission type
- Time-series: Monthly and yearly admission trends
- Correlation analysis: Age, Billing Amount, Length of Stay

### 3. 📈 Visualizations (Python — Matplotlib & Seaborn)
10 charts created covering:

| # | Chart | Type |
|---|---|---|
| 1 | Age Distribution | Histogram with KDE |
| 2 | Avg Billing by Medical Condition | Horizontal Bar |
| 3 | Length of Stay by Admission Type | Box Plot |
| 4 | Test Results by Medical Condition | Stacked Bar (%) |
| 5 | Monthly Admissions Trend | Line Chart |
| 6 | Avg Billing by Insurance Provider | Bar Chart |
| 7 | Correlation Matrix | Heatmap |
| 8 | Medication Usage by Condition | Grouped Bar |
| 9 | Blood Type Distribution | Pie Chart |
| 10 | Age vs Billing by Condition | Facet Grid Heatmap |

### 4. 📋 Excel KPI Dashboard
Built a fully interactive dashboard with:
- **5 KPI Boxes** — Total Patients, Avg Billing, Avg Length of Stay, Avg Age, Abnormal Test Rate
- **5 Pivot Tables** — Billing by condition, patients by insurer, stay by admission type, test results, yearly trend
- **5 Charts** — Bar, Donut, Column, Stacked Column, Line with Markers
- **Slicers** — Dynamic filtering by Medical Condition, Insurance Provider, Admission Type
- **Conditional Formatting** — Test Results (Red/Yellow/Green), Billing Amount (Color Scale), Admission Type (color-coded)

---

## 💡 Key Insights

- **Obesity** had the highest average billing at **$25,860** per patient
- **Emergency admissions** averaged the longest stay at **15.5 days**
- All 5 insurance providers showed nearly **equal patient distribution** (~11,000 each)
- Admissions peaked in **2022** with 11,478 patients before declining
- Test result distribution was relatively **uniform across all medical conditions**

---

## 📊 Dashboard KPIs

| KPI | Value |
|---|---|
| Total Patients | 54,860 |
| Avg Billing Amount | $25,595 |
| Avg Length of Stay | 15.5 days |
| Avg Patient Age | 52 years |
| Abnormal Test Result Rate | ~33% |

---

## 📁 Repository Structure
```
healthcare-analytics/
│
├── data/
│   ├── healthcare_dataset.csv        # Raw dataset
│   └── healthcare_cleaned.xlsx       # Cleaned dataset + Excel Dashboard
│
├── notebooks/
│   └── healthcare_analysis.ipynb     # Full Python analysis & visualizations
│
├── visualizations/
│   └── *.png                         # Exported charts
│
└── README.md
```

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/yourusername/healthcare-analytics.git
```

2. Install dependencies:
```bash
pip install pandas matplotlib seaborn numpy openpyxl
```

3. Open the Jupyter Notebook:
```bash
jupyter notebook notebooks/healthcare_analysis.ipynb
```

4. For the Excel Dashboard, open `data/healthcare_cleaned.xlsx` in Microsoft Excel.

---

## 📬 Contact

Feel free to connect with me on [LinkedIn](https://linkedin.com/in/yourprofile) or reach out via [GitHub](https://github.com/yourusername).

---

*This project was built for portfolio purposes using a synthetic healthcare dataset.*
