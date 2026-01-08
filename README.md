## Project Overview
This project presents an end-to-end exploratory data analysis (EDA) of a healthcare dataset containing patient, clinical, provider, and billing information. The analysis focuses on understanding diagnostic outcomes, **engineered hospital length of stay**, billing patterns, medical conditions, and healthcare service attributes such as doctors, medications, and insurance providers.

The project demonstrates data cleaning, feature engineering, and descriptive statistical analysis in a real-world healthcare setting.

---

## Introduction
In modern healthcare systems, data-driven insights are essential for improving patient outcomes, optimizing hospital operations, and controlling costs. By analyzing diagnostic results alongside hospital stay duration and billing information, healthcare providers can better understand resource utilization and patient care dynamics.

This project applies structured data cleaning, feature engineering, and descriptive statistical analysis to evaluate relationships between different medical details.

---

## Project Objectives
- Engineer **Length of Stay (LOS)** from admission and discharge dates  
- Understand the structure and scope of a multi-dimensional healthcare dataset  
- Explore diagnostic test results and medical conditions  
- Perform descriptive statistics on **billing amount** and LOS  
- Analyze categorical variables such as doctors, medications, and insurance providers  
- Generate actionable insights for healthcare operations and cost management  

---

## 🗂️ Dataset Description
The dataset contains patient-level hospital encounter records with both clinical and administrative information.

### Key Columns
- **Patient name** – Unique patient name 
- **Age** – Patient age  
- **Gender** – Patient gender  
- **Admission Date** – Date of hospital admission  
- **Discharge Date** – Date of hospital discharge  
- **Length of Stay (Days)** – *Derived variable calculated from admission and discharge dates*  
- **Doctor** – Attending or assigned healthcare provider  
- **Medical Condition** – Primary diagnosis (e.g., Asthma)  
- **Test Results** – Diagnostic outcome (Abnormal, Inconclusive, Normal)  
- **Medication** – Prescribed or administered medication(s)  
- **Billing Amount** – Total hospital charges per patient  
- **Insurance Provider** – Patient’s insurance coverage   
- **Admission Type** – Emergency, Urgent, or Elective 

Each row represents a single hospital visit.

---

## 🔍 Understanding the Data
Initial data understanding involved:
- Inspecting dataset dimensions and column data types  
- Differentiating **numerical** and **categorical** features  
- Identifying raw versus engineered columns  
- Reviewing completeness and consistency across clinical and administrative fields  

The dataset represents 10,000 patient records across multiple hospitals over a 5-year period starting from 30-10-2018 to 30-10-2023. There are 10,000 patients in the dataset with 15 columns which contain the patient's details such as name, age, gender, blood group, medical conditions and other details. The minimium age of patient that was admitted is 18 years and maximium is 85 years. The first admission occured on the 30-10-2018 and the last was 30-10-2023.
---

## 🛠️ Data Cleaning & Feature Engineering

### Feature Engineering
- Created **Length of Stay (LOS)** as the difference between discharge and admission dates  

### Numerical Data Cleaning
- Checked for missing, zero and unrealistic values  
-- Explored distributions of:
  - Length of stay  
  - Billing amount  
- Computed summary statistics (mean, median, minimum, maximum)  
- Inspected potential outliers

### Categorical Data Cleaning
- Standardized naming for Doctors, medications, insurance providers and test result categories  
- Verified consistency in medical condition entries  
- Counted frequencies to understand category distribution 

---

## 📊 Exploratory & Descriptive Analysis
- Length of stay showed minimal variation across diagnostic categories.
- Computed mean, median, minimum, and maximum billing amounts  
- Evaluated billing variability across patients  
- Identified cost patterns relevant to hospital resource utilization

 ## Key Insights
 📌 Full insights are documented in
 **README_KEY_INSIGHTS.ipynb

---

## Limitations
- Dataset lacks clinical severity and outcome indicators  
- Medication and billing data do not capture dosage or treatment duration  
- Insurance plans may vary in coverage level despite shared provider names  
- Observational data limits causal inference  

---
 
---

## 🚀 Recommendations & Next Steps
- Analyze LOS and billing by **doctor, department, or insurance provider**  
- Apply statistical testing or regression models  
- Incorporate patient outcomes and comorbidity data  
- Build dashboards for operational decision support  

---

