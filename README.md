# 🚗 U.S. Automotive Recall Analytics

> **Analyzing 25 years of U.S. vehicle recall data to identify safety risks, defect trends, and the growing role of software in automotive reliability.**

**Python • Pandas • Statistical Analysis • Regression • Data Visualization • Automotive Analytics**

---

## 📌 Project Overview

Automotive recalls provide an important signal of **product quality, safety risk, and operational reliability**.

This project analyzes **30K+ NHTSA recall records from 2000–2025** to understand how recall patterns have evolved across manufacturers, defect categories, and safety severity levels.

The analysis focuses on three core questions:

* Which manufacturers generate the largest recall volumes and the highest concentrations of critical safety issues?
* How have automotive defect patterns shifted from **mechanical failures toward software and electronic systems**?
* What trends can help manufacturers and analysts identify emerging product-quality risks?

---

## 🔍 Analytical Workflow

```text
NHTSA Recall Data
       ↓
Data Cleaning & Filtering
       ↓
6,479 Passenger-Vehicle Recalls
       ↓
Text Classification & Feature Engineering
       ↓
Defect Categories + Safety Severity
       ↓
Exploratory & Trend Analysis
       ↓
Regression Modeling
       ↓
Business Insights & Visualization
```

---

## 📊 Data

**Source:** National Highway Traffic Safety Administration (NHTSA)

| Stage                              |   Records |
| ---------------------------------- | --------: |
| Raw recall records                 |    29,663 |
| Passenger-vehicle recalls analyzed |     6,479 |
| Analysis period                    | 2000–2025 |

The raw dataset was cleaned and transformed to isolate recalls relevant to personal passenger vehicles.

Recall descriptions were then converted into structured analytical features including:

* Manufacturer
* Recall year
* Defect category
* Component type
* Safety severity
* Software / electronic vs. mechanical issue

---

## 🧠 Methodology

### 1. Data Preparation

Used Python and Pandas to:

* clean and standardize recall records
* remove irrelevant vehicle categories
* normalize manufacturer information
* process unstructured recall descriptions
* create analysis-ready features

### 2. Defect Classification

Recall descriptions were transformed into structured defect categories such as:

`Airbag` · `Brakes` · `Steering` · `Fuel System` · `Drive Power` · `Software / Electronics` · `High-Voltage Battery`

### 3. Safety Severity Engineering

Developed severity indicators based on safety-critical failure patterns including:

* fire risk
* airbag failure
* steering loss
* braking failure
* loss of drive power
* fuel leakage
* high-voltage battery hazards

This allowed the analysis to move beyond simple recall volume and compare manufacturers based on **risk concentration**.

### 4. Trend & Predictive Analysis

Analyzed long-term recall patterns and applied **linear and polynomial regression** to evaluate the growth of software-related automotive recalls.

---

# 📈 Key Findings

### Ford generated the highest overall recall volume

Across the analyzed passenger-vehicle recalls, Ford recorded the largest number of recall events.

However, recall volume alone does not fully represent safety performance.

---

### Volkswagen showed the highest concentration of critical recalls

When recalls were evaluated using safety-severity indicators rather than total volume, Volkswagen exhibited the highest **criticality rate** among major manufacturers analyzed.

This highlights an important distinction:

> **High recall volume ≠ high safety severity.**

Both metrics are necessary when evaluating manufacturer risk.

---

### 💻 Software is becoming a major automotive reliability risk

Historically, vehicle recalls were dominated by mechanical failures.

The analysis shows software and electronic recalls accelerating over time and **surpassing mechanical recalls by 2023**.

Regression modeling suggests that software-related recalls could reach approximately **2.5× current levels by 2035** if historical trends continue.

This shift reflects a broader transformation in automotive risk:

```text
Mechanical Reliability
        ↓
Electronics Integration
        ↓
Software-Defined Vehicles
        ↓
New Product Quality & Safety Risks
```

---

## 💼 Business Implications

The findings suggest that automotive quality organizations should evaluate recalls using more than total recall counts.

A stronger monitoring framework should combine:

**Recall Volume × Safety Severity × Defect Type × Trend Growth**

For manufacturers and suppliers, increasing software complexity may require greater investment in:

* software quality assurance
* validation and testing
* embedded-system monitoring
* post-release defect detection
* cross-functional engineering risk management

For analysts, separating **recall frequency from recall severity** provides a more useful view of manufacturer product-quality risk.

---

## 🛠️ Skills Demonstrated

**Data Analytics**

* Exploratory Data Analysis
* Trend Analysis
* Business KPI Development
* Data Visualization

**Data Science**

* Feature Engineering
* Text-Based Classification
* Linear Regression
* Polynomial Regression

**Data Engineering**

* Data Cleaning
* Data Transformation
* Structured Analytical Dataset Development

**Business Analysis**

* Problem Framing
* Risk Segmentation
* Manufacturer Benchmarking
* Insight Translation

---

## 🧰 Tech Stack

`Python` `Pandas` `NumPy` `Matplotlib` `Excel` `Tableau`

---

## 📂 Repository Structure

```text
auto-recall-analytics-case/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── data_cleaning.ipynb
│   ├── exploratory_analysis.ipynb
│   └── regression_analysis.ipynb
│
├── visuals/
│
├── presentation/
│
└── README.md
```

---

## 🎯 Project Takeaway

This project demonstrates how unstructured public safety data can be transformed into an analytical framework for evaluating **product quality, manufacturer risk, and emerging automotive technology trends**.

Rather than simply asking **“Who has the most recalls?”**, the analysis asks a more useful business question:

> **Where is automotive safety risk concentrated — and how is that risk changing as vehicles become increasingly software-driven?**
