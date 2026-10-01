# 🏥 Healthcare Data Cleaning, Transformation, Analysis & Visualization

## 📌 Project Overview

This project focuses on **cleaning, transforming, analyzing, and visualizing healthcare data using Microsoft Excel**.

The dataset contains information related to customer/patient details, medical examinations, hospitalization details, health conditions, surgeries, smoking status, BMI, HbA1C, hospital tiers, city tiers, charges, and other healthcare-related attributes.

The main objective of this project is to improve data quality, transform the data into a structured format, perform meaningful analysis, and create visualizations to identify patterns and relationships within the healthcare dataset.

---

## 🎯 Project Objectives

The project covers the following major tasks:

- Identify and handle missing values in the dataset.
- Replace missing values using appropriate strategies such as:
  - Average
  - Mode
  - Default values
  - `Unknown`
- Clean and standardize inconsistent data.
- Split customer names into:
  - Title
  - First Name
  - Last Name
- Convert non-numeric values into appropriate numeric formats.
- Standardize values in columns such as **Heart Issues** and **Smoker**.
- Create **Weight Status** based on BMI.
- Create **Diabetes Status** based on HbA1C values.
- Combine year, month, and date information into a single date column.
- Combine information from multiple tables using **VLOOKUP**.
- Create a consolidated **Healthcare** worksheet.
- Perform data analysis using Excel functions and formulas.
- Create charts and visualizations to present analytical findings.

---

## 🧹 Data Cleaning

The following data-cleaning activities were performed:

### Missing Value Analysis

Missing values represented by `?` were identified in the **Medical Examinations** and **Hospitalization Details** tables.

Missing values were handled using suitable approaches:

- Missing **Month** → Replaced with `Sep`
- Missing **Year** → Replaced using the average year rounded to the nearest integer
- Missing **Smoker** → Replaced with the most frequently occurring value
- Missing **Hospital Tier** → Replaced with the mode
- Missing **City Tier** → Replaced with the mode
- Missing **State ID** → Replaced with `Unknown`

### Data Consistency

The dataset was checked for inconsistent values, particularly in:

- Heart Issues
- Smoker
- Number of Major Surgeries
- Other categorical fields

---

## 🔄 Data Transformation

Several transformations were performed to make the dataset suitable for analysis.

### Customer Name Transformation

The original **Names** column was separated into:

- Title
- First Name
- Last Name

### Number of Major Surgeries

Non-numeric characters were removed and the column was converted into a numeric format.

### Weight Status

A new **Weight Status** column was created using BMI values:

| BMI Range | Weight Status |
|---|---|
| Below 18.5 | Underweight |
| 18.5 – 24.9 | Normal Weight |
| 25.0 – 29.9 | Overweight |
| 30.0 and above | Obesity |

### Diabetes Status

A new **Diabetes Status** column was created using HbA1C values:

| HbA1C Range | Diabetes Status |
|---|---|
| Below 5.7 | Normal |
| 5.7 – 6.4 | Prediabetes |
| 6.5 and above | Diabetes |

### Date Transformation

The available **year, month, and date** information was combined into a single date field for easier analysis.

---

## 🔗 Combining Tables

The different healthcare tables were combined using **VLOOKUP** based on **Customer ID**.

A consolidated worksheet named **Healthcare** was created containing relevant fields such as:

- Customer ID
- First Name
- BMI
- HbA1C
- Heart Issues
- Any Transplants
- Cancer History
- Number of Major Surgeries
- Smoker
- Weight Status
- Diabetes Status
- Date of Birth
- Charges
- Hospital Tier
- City Tier
- State ID
- Age

---

## 📊 Data Analysis & Visualization

The cleaned and consolidated dataset was used to perform several analyses.

### 1. Cancer History Among Smokers and Non-Smokers

The relationship between **smoking status and cancer history** was analyzed using a pie/donut chart.

### 2. Major Surgeries and HbA1C by Transplant History

Patients with and without transplant history were analyzed based on:

- Number of major surgeries
- HbA1C levels

A pie/donut chart was used to present the results.

### 3. Charges by Weight and Diabetes Status

Healthcare charges were analyzed according to:

- Weight Status
- Diabetes Status

A bar chart was created to visualize the differences.

### 4. Average Charges by Hospital Tier Within State

Average healthcare charges were analyzed across different **Hospital Tiers** within states.

A bar chart was used to present the comparison.

### 5. Age, BMI and HbA1C Relationship

The relationship between:

- Age
- BMI
- HbA1C

was analyzed using appropriate charts such as scatter/line charts.

---

## 🛠️ Excel Features & Functions Used

The project makes use of various Microsoft Excel features, including:

- `IF`
- `AVERAGE`
- `ROUND`
- `MODE`
- `VLOOKUP`
- Text-to-Columns
- Find & Replace
- Data Cleaning
- Data Formatting
- Sorting & Filtering
- Conditional Formatting
- Charts
- Pie/Donut Charts
- Bar Charts
- Scatter/Line Charts

---

## 📁 Project File

The main project file included in this repository is:

- **Healthcare Excel Workbook** – Contains the original data, cleaned data, transformed data, consolidated Healthcare sheet, analysis, and visualizations.

If a separate report is included, it explains the **functions, formulas, data-cleaning methods, transformations, and steps performed in Excel**.

---

## 🎓 Learning Outcomes

Through this project, the following Excel and data-analysis skills were practiced:

- Data cleaning and preprocessing
- Missing-value handling
- Data transformation
- Text manipulation
- Excel formulas and functions
- Lookup functions
- Data consolidation
- Healthcare data analysis
- Data visualization
- Dashboard and chart preparation
- Presenting analytical results clearly

---

## 💻 Tools Used

**Microsoft Excel**

The project was completed using Excel's built-in functions, formulas, data-cleaning tools, lookup functions, and visualization features.

---

## 📌 Conclusion

This project demonstrates the complete process of working with a healthcare dataset in Excel, starting from **raw and inconsistent data**, followed by **data cleaning and transformation**, and finally progressing to **analysis and visualization**.

The resulting consolidated dataset provides a structured foundation for examining healthcare-related patterns involving patient characteristics, medical conditions, hospital information, and healthcare charges.
