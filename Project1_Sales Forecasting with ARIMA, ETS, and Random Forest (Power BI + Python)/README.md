# Sales Forecasting with ARIMA, ETS, and Random Forest

Welcome to the Sales Forecasting project repository! This end-to-end project demonstrates how time series and machine learning models can be used to predict daily product sales across various stores. It combines data science and business intelligence tools like Python, Power BI, and GitHub for seamless analytics delivery.

---

## 📊 Business Problem

The goal is to **forecast future sales** across stores and product families using historical data. This helps businesses:

- Anticipate demand
- Manage inventory efficiently
- Plan promotions and operations

---

## 📁 Dataset Overview

The dataset (from [Kaggle's Corporación Favorita dataset](https://www.kaggle.com/competitions/store-sales-time-series-forecasting)) includes:

| File                  | Description                                 |
|-----------------------|---------------------------------------------|
| `train.csv`           | Historical daily sales data                 |
| `test.csv`            | Data for which sales are to be predicted    |
| `oil.csv`             | Daily oil prices                            |
| `stores.csv`          | Store metadata (location, type, cluster)    |
| `transactions.csv`    | Number of transactions per store/day        |
| `holidays_events.csv` | Local, regional, national holidays/events   |
| `sample_submission.csv` | Format for submission                     |

---

## 🔍 Project Pipeline

### 1. 🧹 Data Preparation
- Merged all files into a master dataset.
- Handled missing values (e.g., forward fill for oil prices).
- Enriched with time-based features: `year`, `month`, `dayofweek`, `is_weekend`.

### 2. 📈 Time Series Forecasting
- **ARIMA**: Used for univariate forecasting based on past sales.
- **ETS (Exponential Smoothing)**: Captured trend and seasonality.
- Evaluated using **RMSE**.

### 3. 🤖 Machine Learning
- Trained **Random Forest Regressor** on aggregated and encoded features.
- Achieved the **lowest RMSE**, proving ML outperformed classical methods.

### 4. 📊 Power BI Dashboard
Built a 5-page interactive Power BI report covering:
1. Overview & Business Problem
2. Data Exploration
3. Time Series Forecasts (ARIMA & ETS)
4. Machine Learning Results (Random Forest)
5. Final Recommendations

---

## 📈 Model Performance (RMSE)

| Model        | RMSE         |
|--------------|--------------|
| ARIMA        | 107,251.00   |
| ETS          | 161,663.76   |
| **Random Forest** | **371.08** ✅ Best |

---

## 📦 Repository Structure

```bash
Cloudcredits/
├── Sales_Forecasting_ARIMA_ETS_RF.ipynb         # Main Python notebook
├── forecast_summary.csv                          # ARIMA & ETS Forecast (Power BI Page 3)
├── rf_predictions.csv                            # Random Forest Forecast (Page 4)
├── rf_feature_importance.csv                     # Feature Importance (Page 4)
├── submission.csv / test_predictions.csv         # Final predictions for test set
├── train_enriched_sample.csv                     # Feature-engineered sample (<25MB) for dashboard
├── Sales_Forecasting_Project_Report_Eyesly.pdf   # 📘 Full project report (PDF)
├── README.md                                     # 🔍 This file
├── .gitignore                                     # Git ignore rules
├── LICENSE                                       # MIT License
🚀 Tools & Technologies
Tool	Purpose
Python	Data analysis and modeling
Pandas	Data manipulation
statsmodels	ARIMA, ETS modeling
scikit-learn	Machine learning (Random Forest)
Power BI	Dashboard and visualization
Git & GitHub	Version control and collaboration

📈 Power BI Dashboard Link
You can view or download the full Power BI dashboard here:
🔗 https://drive.google.com/drive/u/0/folders/1SA_Tl1PJRE7xYKICO3M07leajcOfvjiT

📄 Project Report
A complete project report is included in this repository.
📘 Download PDF Report

It covers everything — from data enrichment, model performance, insights, to recommendations. Highly recommended for recruiters and mentors.

👩‍💻 Author
Eyesly Meribha Johnson Paulraj
📍 Data Scientist | MSc in Data Science | Power BI & ML Expert
🔗 linkedin.com/in/eyesly-meribha-johnson-paulraj-7a8b49221

📄 License
This project is licensed under the MIT License.

🙋‍♀️ For Recruiters & Reviewers
This project reflects my hands-on ability in:

Data wrangling & exploration

Time Series Forecasting

Machine Learning modeling

Dashboard storytelling via Power BI

GitHub documentation

Please feel free to explore this repository, or reach out via LinkedIn for collaboration or hiring opportunities.
