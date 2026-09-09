# 🚗 U.S. Automotive Recall Analytics

<p align="center">

<img src="https://img.shields.io/badge/Python-Data%20Analytics-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Pandas-Data%20Wrangling-150458?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/scikit--learn-Regression-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
<img src="https://img.shields.io/badge/NHTSA-Public%20Safety%20Data-005EA8?style=for-the-badge" />
<img src="https://img.shields.io/badge/Excel-Analysis-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" />

</p>

<p align="center">
  <strong>25 Years of Automotive Safety Intelligence</strong><br>
Manufacturer benchmarking, defect-risk analysis, and recall trend modeling using 29K+ NHTSA records.
</p>

> **What if recall volume alone is hiding where the real automotive safety risk is?**
>
> This project transforms 25 years of U.S. automotive recall data into structured defect categories, safety-severity indicators, manufacturer benchmarks, and predictive trend insights to understand how vehicle reliability is evolving from mechanical failures toward software-driven risk.

<img src="automotive-recall-analytics.png" width="100%" />

---

## 🧠 What This Analysis Does

The project answers four core business questions:

| Question                                                                  | Analytical Approach                       |
| ------------------------------------------------------------------------- | ----------------------------------------- |
| *Which manufacturers generate the most recalls?*                          | Manufacturer benchmarking                 |
| *Which manufacturers have the highest concentration of critical defects?* | Safety severity analysis                  |
| *What types of failures are driving automotive recalls?*                  | Text classification + feature engineering |
| *How is recall risk changing as vehicles become more software-driven?*    | Trend analysis + regression modeling      |

---

## 🏗️ Analytics Architecture

<img src="recall-analytics-architecture.png" width="100%" />

```text
NHTSA Recall Data
        ↓
Data Cleaning & Filtering
        ↓
Passenger Vehicle Dataset
        ↓
Text Classification
        ↓
Feature Engineering
        ↓
Safety Severity Scoring
        ↓
EDA & Manufacturer Benchmarking
        ↓
Regression Modeling
        ↓
Power BI Insights
```

---

## 🔄 Data Pipeline

Built to transform raw recall records into an analytics-ready dataset for business intelligence and predictive analysis.

### 📥 Raw Data

Started with **29,663 NHTSA recall records** covering model years and recall activity from **2000–2025**.

### 🧹 Cleaning & Filtering

Filtered and standardized the dataset to isolate:

**6,479 passenger-vehicle recall records**

Cleaning included:

* Manufacturer standardization
* Vehicle-type filtering
* Missing-value treatment
* Duplicate review
* Text normalization
* Date and category transformation

### 🧠 Feature Engineering

Unstructured recall descriptions were converted into structured analytical features including:

`Manufacturer` · `Defect Category` · `Severity Level` · `Component Type` · `Mechanical / Software`

Safety-critical indicators captured issues related to:

🔥 **Fire**
🎈 **Airbags**
🛞 **Steering**
🛑 **Brakes**
⛽ **Fuel Leakage**
🔋 **High-Voltage Battery**
⚙️ **Loss of Drive Power**

---

## 📊 Manufacturer & Safety Analysis

Recall volume alone does not fully represent product risk.

This project evaluates manufacturers from two different perspectives:

| Metric               | Business Meaning                                                  |
| -------------------- | ----------------------------------------------------------------- |
| **Recall Volume**    | How frequently a manufacturer experiences recall events           |
| **Criticality Rate** | How concentrated those recalls are in high-severity safety issues |

### Key Result

**Ford** recorded the highest overall recall volume in the analyzed dataset.

However, **Volkswagen** showed the highest concentration of critical recalls among major manufacturers analyzed.

```text
High Recall Volume
        ≠
High Safety Severity
```

This distinction allows manufacturer performance to be evaluated beyond simple recall counts.

---

## ⚙️ Defect Intelligence

Recall descriptions were categorized to identify how product failures are changing over time.

The analysis compares traditional mechanical failures against emerging software and electronic issues.

### Automotive Reliability Shift

```text
Mechanical Systems
        ↓
Electronic Systems
        ↓
Connected Vehicles
        ↓
Software-Defined Vehicles
        ↓
New Reliability Risks
```

One of the strongest patterns in the dataset was the increasing contribution of **software and electronic defects** to total recall activity.

---

## 🤖 Trend Modeling

### Software Recall Growth

Linear and polynomial regression were used to evaluate the historical growth of software-related recalls.

The modeling pipeline:

```text
Historical Recall Data
        ↓
Software Recall Classification
        ↓
Year-Level Aggregation
        ↓
Trend Feature Engineering
        ↓
Linear + Polynomial Regression
        ↓
Future Recall Projection
```

### Key Finding

Software/electronic recalls surpassed mechanical recalls by **2023** within the analyzed dataset.

Historical trend modeling suggests software-related recalls could grow to approximately:

# **2.5× by 2035**

if the observed historical trajectory continues.

> The projection is intended as a trend scenario rather than a deterministic forecast.

---

## 📈 Key Insights

### 🥇 Ford — Highest Recall Volume

Ford generated the highest number of recall events among the manufacturers analyzed.

This indicates significant recall exposure but does not automatically imply the highest safety risk.

---

### ⚠️ Volkswagen — Highest Criticality Rate

Volkswagen showed a greater concentration of recalls associated with high-severity safety categories.

This demonstrates why **severity-adjusted analysis** provides additional information beyond total recall counts.

---

### 💻 Software Risk Is Accelerating

Software and electronics represent an increasingly important source of vehicle reliability risk.

As vehicles become more software-defined, traditional manufacturing quality controls may need to expand toward:

* Software validation
* Embedded-system testing
* OTA update governance
* Post-release monitoring
* Cross-functional engineering risk management

---

## 💡 Business Intelligence Framework

The project reframes automotive recall analysis around four dimensions:

```text
Recall Risk
    │
    ├── Volume
    │
    ├── Severity
    │
    ├── Defect Type
    │
    └── Trend Growth
```

Instead of asking only:

> **“Which manufacturer has the most recalls?”**

the project asks:

> **“Where is product safety risk concentrated, what is causing it, and how is that risk changing over time?”**

---

## 📊 Power BI Dashboard

The dashboard translates the analytical dataset into interactive manufacturer and defect intelligence.

### Core Views

| View                           | Description                                                           |
| ------------------------------ | --------------------------------------------------------------------- |
| 🏭 **Manufacturer Overview**   | Compare recall volume across major automotive manufacturers           |
| ⚠️ **Safety Severity**         | Identify manufacturers with higher concentrations of critical recalls |
| 🔧 **Defect Analysis**         | Explore recall patterns by component and failure category             |
| 💻 **Software vs. Mechanical** | Track the shift in recall composition over time                       |
| 📈 **Trend Intelligence**      | Visualize historical patterns and long-term recall growth             |

```text
Processed Recall Data
          ↓
Analytical KPIs
          ↓
Manufacturer & Defect Analysis
          ↓
Trend Modeling
          ↓
Interactive Power BI Dashboard
```

---

## 🛠️ Tech Stack

### Analytics & Data Science

`Python` `Pandas` `NumPy` `scikit-learn`

### Business Intelligence

`Power BI` `Excel`

### Analytical Methods

`EDA` `Feature Engineering` `Text Classification` `Trend Analysis` `Linear Regression` `Polynomial Regression`

### Data Source

`National Highway Traffic Safety Administration — NHTSA`

---

## 📁 Project Structure

```text
auto-recall-analytics-case/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   ├── raw/
│   │   └── ...                 # Original NHTSA recall data
│   │
│   └── processed/
│       └── ...                 # Cleaned analytics-ready datasets
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_defect_classification.ipynb
│   ├── 03_exploratory_analysis.ipynb
│   └── 04_regression_modeling.ipynb
│
├── src/
│   └── ...                     # Reusable analysis / transformation scripts
│
├── visuals/
│   └── ...                     # Charts and analytical outputs
│
├── dashboard/
│   └── ...                     # Power BI dashboard assets
│
└── automotive-recall-analytics.png
```

---

## 🎯 Project Takeaway

Automotive recall risk is no longer purely a **mechanical reliability problem**.

The growing role of software and electronics introduces a new layer of product-quality risk that requires manufacturers to evaluate not only **how often failures occur**, but also:

**how severe they are, what systems they affect, and how quickly those risks are evolving.**

---

## 👤 Author

**Thinh Nguyen**

Data Analytics / Data Science / Analytics Engineering

---

<div align="center">

**Turning public safety data into product-risk intelligence.**

</div>
