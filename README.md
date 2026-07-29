# Capstone Project, 44688-80
# Author: Brenda Fuemmeler
# Date: Summer 2026


# Predicting Hospital Quality Outcomes Using CMS Hospital Compare Data

## Project Overview

This project develops machine learning models to predict hospital quality ratings using publicly available data from the Centers for Medicare & Medicaid Services (CMS) Hospital Compare program.

The objective is to determine whether hospital characteristics, patient experience measures, infection rates, mortality outcomes, and readmission rates can accurately predict CMS Hospital Overall Ratings.

The project follows a complete data science workflow including:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Predictive Modeling
- Model Evaluation
- Interactive Dashboard Development

---

# Research Question

**Can machine learning accurately predict CMS Hospital Overall Ratings using publicly available hospital quality measures?**

---

# Dataset

Source:

- CMS Hospital Compare
- HealthData.gov

Datasets included:

- Hospital General Information
- HCAHPS Patient Experience
- Hospital Infections
- Hospital Mortality
- Hospital Readmissions

---

# Repository Structure

```text
capstone-hospital-quality/
│
├── data/
│   ├── raw/
│   ├── interim/
│   ├── processed/
│   └── external/
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_EDA.ipynb
│   ├── 04_predictive_modeling.ipynb
│   └── 05_model_evaluation.ipynb
│
├── reports/
│
├── references/
│
├── src/
│
├── README.md
├── pyproject.toml
├── requirements.txt
└── LICENSE
```

---

# Project Progress

## Phase 1 — Data Collection

Downloaded publicly available CMS Hospital Compare datasets and organized them within the project structure.

Datasets include:

- Hospital General Information
- HCAHPS
- Hospital Infections
- Hospital Mortality
- Hospital Readmissions

---

## Phase 2 — Data Cleaning

Completed the following cleaning tasks:

- Verified file formats
- Detected delimiters automatically
- Removed duplicate records
- Standardized Facility ID data types
- Examined missing values
- Verified data quality
- Saved cleaned datasets to the `data/interim` directory

---

## Phase 3 — Exploratory Data Analysis (EDA)

Performed exploratory analysis to understand the structure and quality of each dataset.

EDA included:

- Dataset summaries
- Data type verification
- Missing value analysis
- Summary statistics
- Distribution of hospital ratings
- Geographic distribution of hospitals
- Dataset validation

---

## Feature Engineering

A major portion of this project involved transforming CMS measure-level datasets into hospital-level analytical features.

### HCAHPS

Selected seven patient experience star-rating measures:

- Nurse Communication
- Doctor Communication
- Cleanliness
- Quietness
- Communication About Medicines
- Discharge Information
- Recommend Hospital

These measures were pivoted to create one row per hospital.

---

### Hospital Infections

Selected six Standardized Infection Ratio (SIR) measures:

- Central Line Bloodstream Infection
- Catheter Associated Urinary Tract Infection
- Colon Surgery SSI
- Hysterectomy SSI
- MRSA
- Clostridium difficile

These measures were pivoted into hospital-level features.

---

### Hospital Mortality

Selected six condition-specific mortality measures:

- Heart Attack
- CABG
- COPD
- Heart Failure
- Pneumonia
- Stroke

These variables were transformed into one record per hospital.

---

### Hospital Readmissions

Selected six condition-specific readmission measures:

- Heart Attack
- CABG
- COPD
- Heart Failure
- Hip/Knee Replacement
- Pneumonia

These variables were pivoted into hospital-level features.

---

## Master Dataset

The final analytical dataset contains approximately:

- **5,432 hospitals**
- Hospital characteristics
- Patient experience measures
- Infection measures
- Mortality measures
- Readmission measures

Each row represents one hospital and is ready for predictive modeling.

---

# Current Status

Completed:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Master Dataset Construction

In Progress:

- Predictive Modeling

Upcoming:

- Model Evaluation
- Feature Importance Analysis
- Power BI Dashboard
- Final Report

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Git
- GitHub
- Power BI
- LaTeX

---

# Expected Machine Learning Models

Planned models include:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost (if applicable)

Models will be evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix

---

