# Sales & Demand Forecasting 

This repository contains my implementation for **Machine Learning Task 1**, focused on building a **business-oriented sales forecasting system** using historical time-series data.

The goal is not only to train a model, but to demonstrate how Machine Learning supports real business decision-making.

---

## 🎯 Project Objective

The objective of this project is to:

- Predict future sales based on historical patterns
- Understand trends and seasonality in time-series data
- Build a forecasting pipeline using Machine Learning
- Present results in a clear, business-friendly way

This project simulates how companies forecast demand to support inventory, staffing, and financial planning.

---

## 📊 Dataset

**Kaggle Competition:**  
Store Sales — Time Series Forecasting

The dataset contains historical daily sales across multiple stores and product categories.

For this project:
- Total daily sales were aggregated to represent overall business demand.
- Time-based features were created to capture seasonality and trends.

---

## ⚙️ Project Workflow

### 1️⃣ Data Preparation
- Loaded historical sales data
- Converted date column to datetime format
- Aggregated daily sales
- Handled missing dates using daily frequency

---

### 2️⃣ Feature Engineering (Time Series)
Created features to help the model understand patterns:

**Time-based features**
- Day of week
- Month
- Day
- Year
- Weekend indicator

**Lag Features**
- Previous day sales (lag_1)
- Previous week sales (lag_7)

**Rolling Features**
- 7-day moving average
- 30-day moving average

These features help capture trend and seasonality.

---

### 3️⃣ Forecasting Model

Model Used:
HistGradientBoostingRegressor (Scikit-learn)

Why this model?
- Works well on structured tabular data
- Handles non-linear relationships
- Fast and robust baseline for business forecasting

---

### 4️⃣ Model Evaluation

Performance measured using:

- MAE — Mean Absolute Error
- RMSE — Root Mean Squared Error
- MAPE — Mean Absolute Percentage Error

These metrics help evaluate how reliable forecasts are for business planning.

---

### 5️⃣ Visualization (Business Focused)

Clear charts were created for non-technical stakeholders:

- Actual vs Predicted Sales
- Historical Trend Analysis
- 30-Day Future Forecast

The goal is to communicate insights clearly to managers or business owners.

---

## 📈 Business Value

This forecasting system can help businesses:

- 📦 Plan inventory levels
- 👥 Optimize staffing decisions
- 💰 Forecast revenue and cash flow
- 📅 Understand seasonal demand patterns
- 📉 Reduce overstocking or shortages

---

## 📂 Repository Structure

Sales & Demand Forecasting/
├── notebooks/
│ └── Task1_StoreSales_Forecast.ipynb
├── outputs/
│ ├── forecast_plot.png
│ ├── actual_vs_predicted.png
│ └── forecast_next_30_days.csv
├── requirements.txt
└── README.md


---

## 🚀 How to Run This Project

### 1️⃣ Clone the repository
git clone https://github.com/farid-doy10/FUTURE_ML_01.git


### 2️⃣ Install dependencies
pip install -r requirements.txt


### 3️⃣ Open the Notebook
notebooks/Task1_StoreSales_Forecast.ipynb

---

## 🧰 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 🔮 Future Improvements

- Include holidays and oil price features
- Forecast per store or product category
- Compare multiple time-series models
- Deploy interactive dashboard (Power BI / Streamlit)

---


---

## 👤 Author

Ahmed Farid Al Basir
