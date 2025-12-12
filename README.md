# Predictive Analytics of School Performance in Saudi Arabia

This repository presents an end-to-end data science and analytics project focused on analyzing and predicting school performance in Saudi Arabia using educational performance data.

The project combines data cleaning, exploratory analysis, machine learning models, and an interactive dashboard to support data-driven insights into school outcomes across regions, cities, and exam types.

---

## Project Overview

The project addresses the following analytical and modeling tasks:

- Cleaning and preprocessing school performance data
- Exploratory Data Analysis (EDA) of scores, rankings, and geographic distributions
- Predictive modeling using supervised and unsupervised learning
- Interactive visualization through a Streamlit dashboard

---

## Machine Learning Models

The following models and techniques are implemented:

### 1. Regression
- **Linear Regression** to predict school average scores
- Uses only **previous-year features** to avoid data leakage
- Evaluated using R² and Mean Absolute Error (MAE)

### 2. Classification
- **Binary classification** to identify **top 10% performing schools**
- Based on national ranking thresholds
- Evaluated using accuracy, precision, recall, F1-score, and confusion matrix

### 3. Logistic Regression
- Classifies schools as **underperforming vs not underperforming**
- Based on comparison between school average score and area average
- Includes ROC curve and AUC evaluation

### 4. Unsupervised Learning
- **Principal Component Analysis (PCA)** on performance-related features
- Used to reduce dimensionality and explore latent performance patterns
- Visualized using PCA scatter plots

---

## Interactive Dashboard

An interactive dashboard was developed using **Streamlit** to allow dynamic exploration of the data and model results.

### Dashboard features include:
- Filtering by year, region, city, authority, education type, exam type, and specialization
- Key performance indicators (KPIs)
- Interactive charts (bar charts, scatter plots)
- Geographic visualization of schools on a map
- School-level detailed views
- On-demand execution of machine learning models

---

## Files in This Repository

- `PresentationDashboard.py`  
  Streamlit application containing data exploration, visualizations, and machine learning models.

- `.csv`  
  Raw school performance dataset used by the dashboard.

---

## How to Run the Dashboard

1. Install required libraries:
   ```bash
   pip install pandas numpy scikit-learn streamlit altair
