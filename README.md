<<<<<<< HEAD
# FUTURE_ML_01 — Sales & Demand Forecasting (Time Series)

## Program
Future Interns — Machine Learning Track (ML)

## Objective
Build a sales/demand forecasting system using historical time-series data and present results in a business-friendly way.

## Dataset
Kaggle Competition: Store Sales — Time Series Forecasting

## Approach Summary
- Loaded `train.csv` and converted `date` to datetime
- Aggregated total daily sales across all stores and product families
- Cleaned data (handled missing dates by daily frequency and filling)
- Engineered time-based features (day-of-week, month, year, weekend)
- Added lag features and rolling averages (trend + seasonality signals)
- Trained a machine learning model for forecasting
- Evaluated performance using MAE, RMSE, and MAPE
- Produced clear visualizations and a 30-day future forecast

## Repository Structure
=======
# FUTURE_ML_01 — Sales & Demand Forecasting (Machine Learning Internship Task)

## Internship
Future Interns — Machine Learning Track (ML)

This repository contains my implementation for **Machine Learning Task 1**, focused on building a **business-oriented sales forecasting system** using historical time-series data.

---

## Project Objective

The goal of this project is to predict future sales based on historical patterns and present results in a clear, business-friendly format.

Instead of focusing only on model accuracy, this project demonstrates:

- Time-series data preparation
- Feature engineering using dates and trends
- Forecasting using machine learning
- Business interpretation of predictions
- Visualization for non-technical stakeholders

---

## Dataset

Kaggle Competition:
Store Sales — Time Series Forecasting

The dataset contains historical daily sales from multiple stores and product families.

For this task, total daily sales were aggregated to simulate a real business revenue forecasting scenario.

---

## Project Workflow

### 1. Data Preparation
- Converted date column to datetime format
- Aggregated total sales per day
- Filled missing dates using daily frequency
- Checked for missing values

### 2. Time-Based Feature Engineering
Created features to capture trend and seasonality:

- Day of week
- Month
- Day
- Year
- Weekend indicator

Lag-based features:
- Previous day sales (lag_1)
- Previous week sales (lag_7)
- Rolling averages (7-day and 30-day)

These features help the model learn temporal patterns.

---

### 3. Forecasting Model

Model Used:
HistGradientBoostingRegressor (Scikit-learn)

Reason:
- Strong performance on structured data
- Handles non-linear relationships
- Suitable baseline for business forecasting

---

### 4. Model Evaluation

Evaluation Metrics:

- MAE — Mean Absolute Error
- RMSE — Root Mean Squared Error
- MAPE — Mean Absolute Percentage Error

These metrics help measure prediction reliability for business planning.

---

### 5. Visualization

Business-friendly plots were created:

- Actual vs Predicted Sales
- Historical Trend Analysis
- Future 30-Day Forecast

Goal:
Ensure non-technical stakeholders can understand insights easily.

---

## Business Impact

This forecasting system can help businesses:

- Plan inventory levels
- Manage staffing requirements
- Estimate revenue and cash flow
- Identify seasonal demand patterns
- Reduce overstocking or shortages

---

## Repository Structure

>>>>>>> 6988199d842168e95ec9171b1aada4b946dc60a7
