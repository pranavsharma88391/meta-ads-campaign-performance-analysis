# 📊 Meta Ads Campaign Performance Analysis

## 📌 Project Overview
This project presents an end-to-end analytical evaluation of Meta (Facebook & Instagram) advertising campaigns. Using **Python**, **Statistical Analysis**, and **Power BI**, the analysis assesses ad spend, impressions, clicks, conversions, and revenue to uncover performance patterns across campaigns, platforms, and regions. 

The primary objective is to identify high-performing ad segments, detect cost anomalies, and deliver data-backed recommendations for marketing budget reallocation and Return on Ad Spend (ROAS) optimization.

---

## 🎯 Key Objectives
- **Data Cleaning & Integrity:** Standardize raw campaign logs, handle missing values, remove duplicate records, and validate data types[cite: 22].
- **KPI Modeling:** Compute core digital marketing metrics including **CTR**, **CPC**, **CPM**, **CPA**, and **ROAS**[cite: 22].
- **Statistical & Outlier Analysis:** Apply descriptive statistics, correlation matrices, and the **Interquartile Range (IQR)** method to detect abnormal spend or conversion spikes[cite: 22].
- **Visual Storytelling:** Build an interactive Power BI dashboard for comparative reporting across regions, platforms, and campaign objectives[cite: 22].

---

## 🛠️ Tech Stack & Tools
- **Programming Language:** Python 3.x[cite: 22]
- **Data Manipulation & Analysis:** Pandas, NumPy, SciPy, Stats[cite: 22]
- **Data Visualization:** Matplotlib, Seaborn, Power BI (DAX, Power Query)[cite: 22]
- **Environment:** Jupyter Notebook / VS Code

---

## 🔍 Analytical Workflow

### 1. Data Preprocessing & Quality Checks
- Inspected schema, data types, and summary statistics across raw campaign exports.
- Handled null/missing values, eliminated duplicate entries, and standardized date and categorical fields using `Pandas`[cite: 22].

### 2. Marketing KPI Calculations
Engineered key campaign efficiency metrics:
- **CTR (Click-Through Rate):** `(Clicks / Impressions) * 100`
- **CPC (Cost Per Click):** `Total Spend / Total Clicks`
- **CPM (Cost Per Mille):** `(Total Spend / Impressions) * 1000`
- **CPA (Cost Per Acquisition):** `Total Spend / Total Conversions`
- **ROAS (Return on Ad Spend):** `Total Revenue / Total Spend`

### 3. Exploratory Data Analysis (EDA) & Statistical Testing
- Evaluated campaign performance segmented by **Platform**, **Target Region**, and **Campaign Type**[cite: 22].
- Conducted **Correlation Analysis** to measure relationships between ad spend, click volume, and conversion revenue[cite: 22].
- Implemented **IQR-Based Outlier Detection** (`Q1 - 1.5*IQR` and `Q3 + 1.5*IQR`) to isolate underperforming high-spend outliers and anomalous traffic spikes[cite: 22].

### 4. Power BI Interactive Dashboard
- Transformed cleaned datasets using **Power Query** and created dynamic measures using **DAX**[cite: 22].
- Designed comparative visuals highlighting regional ROI, platform-wise conversion funnels, and cost-per-acquisition trends[cite: 22].

---

## 💡 Business Recommendations
- **Reallocate Budget to High-ROAS Segments:** Shift ad spend away from high-CPA, low-converting campaigns toward top-performing platform-region combinations[cite: 22].
- **Cap Outlier Spend:** Set automated bid and daily budget caps on campaigns flagged by IQR outlier analysis where increased spend yielded diminishing returns[cite: 22].
- **Optimize Underperforming Creatives:** Review campaigns with high impressions (low CPM) but low CTR to improve ad copy and audience targeting[cite: 22].

---

## 📂 Repository Structure
```text
├── data/                   # Raw and cleaned campaign datasets (CSV/Excel)
├── notebooks/              # Jupyter notebooks for data cleaning, EDA, and IQR stats
├── dashboard/              # Power BI (.pbix) file and dashboard screenshots
├── reports/                # Executive summary and business recommendations
└── README.md               # Project documentation
