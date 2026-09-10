# Excel-Capstone-Project---MODULE-1

## AI-Powered Healthcare Data Insights and Dashboarding

## 📌 Project Overview

This project focuses on analyzing healthcare data using **Microsoft Excel** to identify meaningful insights related to patient health profiles, medical history, hospitalisation details, and healthcare costs.

The project demonstrates the complete data analytics workflow, including:

- Data Cleaning
- Data Transformation
- Data Preparation
- Exploratory Data Analysis
- Pivot Tables
- Data Visualization
- AI-Powered Summary Statistics
- Interactive Dashboard Creation

- The objective is to transform raw healthcare data into meaningful insights that can support healthcare providers and policymakers in understanding patient profiles, healthcare costs, and health-related patterns.

---

## 🎯 Problem Statement

The healthcare industry generates large volumes of data from medical examinations, hospitalisation records, and customer profiles.

This project analyzes a comprehensive healthcare dataset to:

- Understand patient health profiles
- Analyze medical histories
- Explore healthcare costs
- Identify relationships between health metrics
- Analyze cancer history and smoking patterns
- Categorize patients based on BMI
- Visualize healthcare statistics
- Build an interactive healthcare dashboard


## 🗂️ Dataset

The dataset consists of three main tables:

### 1. Medical Examinations
Contains medical and health-related information such as:

- Customer ID
- BMI
- HBA1C
- Heart Issues
- Any Transplants
- Cancer History
- Number of Major Surgeries
- Smoker

### 2. Hospitalization Details
Contains hospitalisation-related information such as:

- Customer ID
- Year
- Month
- Date
- Charges
- Hospital Tier
- City Tier
- State ID

### 3. Customer Names
Contains customer information including:

- Customer ID
- Names

- 
# 🧹 Data Cleaning

The following data-cleaning activities were performed:

### Missing Value Analysis

Missing values represented by `?` were identified in the Medical Examinations and Hospitalization Details tables.

### Missing Month

Missing values in the `month` column were replaced with:

`Sep`

### Missing Year

Missing values in the `year` column were replaced using the average year rounded to the nearest integer.

### Mode Imputation

The most frequently occurring values were identified for:

- Smoker
- Hospital Tier
- City Tier

Missing values were filled using the respective mode.

### State ID

Missing State ID values were handled using:

`Unknown`

where appropriate.

---

# 🔄 Data Transformation

### 1. Customer Name Transformation

The `names` column was split into three separate columns:

- Title
- First Name
- Last Name

### 2. Number of Major Surgeries

The `NumberOfMajorSurgeries` column was converted into numerical data by replacing non-numeric/missing characters with appropriate numerical values.

### 3. Data Consistency Checks

The following columns were checked for inconsistencies:

- Heart Issues
- Smoker

Corrective actions were applied where required to maintain consistent categorical values.

### 4. Weight Status

A new column called `Weight Status` was created using BMI values.

| BMI Range | Weight Status |
|---|---|
| Below 18.5 | Underweight |
| 18.5 – 24.9 | Normal Weight |
| 25.0 – 29.9 | Overweight |
| 30.0 and Above | Obesity |

### 5. Date of Birth

The following columns were merged:

- Year
- Month
- Date

A new `Date of Birth` column was created and formatted as:

`DD-MMM-YYYY`

### 6. Age Calculation

Customer age was calculated using the dataset collection date:

**8 June 2023**

### 7. Charges Formatting

The `charges` column was formatted as currency:

**$**

---

# 📊 Healthcare Dataset

A new worksheet named **Healthcare** was created by combining the three source tables using **Customer ID** as the common key.

The final dataset contains the following 17 columns:

1. Customer ID
2. First Name
3. BMI
4. HBA1C
5. Heart Issues
6. Any Transplants
7. Cancer History
8. Number of Major Surgeries
9. Smoker
10. Weight Status
11. Diabetes Status
12. Date of Birth
13. Charges
14. Hospital Tier
15. City Tier
16. State ID
17. Age

---

# 📈 Pivot Table Analysis

Pivot Tables were created to explore relationships within the healthcare dataset.

The analysis includes:

- Cancer history among smokers and non-smokers
- Distribution of healthcare costs by weight status
- Patient and hospitalisation statistics
- Healthcare cost analysis
- Medical metric summaries

---

# 📊 Data Visualization

The project includes multiple visualizations created using Microsoft Excel.

### 🍩 Cancer History vs Smoker

A Pie/Donut chart was created to analyze the distribution of cancer history among:

- Smokers
- Non-smokers

### 📊 Charges by Weight Status

A Column Chart was created to compare healthcare charges across different weight-status categories:

- Underweight
- Normal Weight
- Overweight
- Obesity

### 📊 Summary Statistics

Quick Analysis and Recommended Charts were used to visualize overall healthcare statistics, including:

- Total Customers
- Total Hospitalisations
- Total Healthcare Costs
- Average Healthcare Costs
- Average Medical Metrics

---

# 🤖 AI-Powered Analysis

Excel's **Quick Analysis** and **Recommended Charts** features were used to automatically generate summary statistics and visualizations.

This helped identify important patterns and distributions within the healthcare dataset.

---

# 📋 Dashboard

An interactive **Healthcare Dashboard – AI Analysis** was created to consolidate the major findings.

The dashboard includes:

- Cancer History vs Smoker visualization
- Charges by Weight Status
- Healthcare summary statistics
- Recommended charts
- Weight Status slicer
- Diabetes Status slicer

The dashboard was designed with a simple and consistent layout for easy interpretation.

---

# 🔍 Key Insights

The analysis provides insights into:

- Distribution of cancer history among smokers and non-smokers
- Healthcare charges across different BMI categories
- Overall number of customers and hospitalisations
- Average healthcare costs
- Patient medical characteristics
- Distribution across hospital and city tiers
- Relationships between different healthcare indicators

---

# 🛠️ Tools & Technologies

- **Microsoft Excel**
- Pivot Tables
- Pivot Charts
- Quick Analysis
- Recommended Charts
- XLOOKUP
- Excel Formulas
- Conditional Formatting
- Slicers
- Data Cleaning & Transformation

---
