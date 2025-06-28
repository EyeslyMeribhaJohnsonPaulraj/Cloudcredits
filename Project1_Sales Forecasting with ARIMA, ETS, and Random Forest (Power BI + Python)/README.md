# Sales Forecasting with ARIMA, ETS, and Random Forest

A full-stack data science project that demonstrates advanced time series forecasting using classical models (ARIMA, ETS) and machine learning (Random Forest), along with a professional Power BI dashboard.

---

## Business Problem

Retail businesses struggle with accurately forecasting product demand across locations and time. This project forecasts **daily sales** using time series data from Ecuadorian stores.

Accurate forecasting helps in:
- Inventory management
- Promotions & planning
- Operational cost reduction

---

## 📁 Dataset Overview

This project uses historical sales data enriched with:
- 🛢️ Oil prices (`oil.csv`)
- 🏖️ Holiday events (`holidays_events.csv`)
- 🏬 Store information (`stores.csv`)
- 🧾 Transactions (`transactions.csv`)

---

## 🔍 Methodology

### 1. Data Enrichment
Combined multiple datasets into one feature-rich training set.

### 2. Feature Engineering
Created features like:
- `year`, `month`, `dayofweek`, `is_weekend`
- Aggregations on transactions and oil prices

### 3. Forecasting Models
- **ARIMA** (Auto Regressive Integrated Moving Average)
- **ETS** (Exponential Smoothing)
- **Random Forest** Regressor

### 4. Model Evaluation (RMSE)

| Model          | RMSE (Lower is better) |
|----------------|------------------------|
| ARIMA          | 107,251.00             |
| ETS            | 161,663.76             |
| Random Forest  | **264.01** ✅ Best     |

---

## 📈 Power BI Dashboard

Interactive 5-page dashboard designed for business stakeholders:

1. **Overview & KPIs** — Sales, stores, product families  
2. **Data Exploration** — Sales by store, family, trends  
3. **ARIMA/ETS Forecast** — Visual + RMSE comparison  
4. **RF Forecast** — Actual vs Predicted, Feature Importance  
5. **Final Insights** — Recommendations for the business  

---

## 📸 Dashboard Visuals

These visuals are available in the GitHub repository under `dashboard_visuals/`:

| Page | Description                          |
|------|--------------------------------------|
| 1    | Overview & Business Problem          |
| 2    | Data Exploration                     |
| 3    | ARIMA & ETS Forecasting              |
| 4    | Random Forest Forecast               |
| 5    | Final Submission & Insights          |

---

## 📦 Repository Contents

| File                                      | Purpose                                                    |
|-----------------------------------------------|--------------------------------------------------------|
| `Sales_Forecasting_ARIMA_ETS_RF.ipynb`        | Main Jupyter notebook with full code                   |
| `forecast_summary.csv`                        | Output of ARIMA/ETS predictions for dashboard          |
| `rf_predictions.csv`                          | Random Forest predictions                              |
| `rf_feature_importance.csv`                   | Feature importance from RF                             |
| `submission.csv` / `test_predictions.csv`     | Final predictions for test data                        |
| `train_enriched_sample.csv`                   | Feature-engineered sample (<25MB) for dashboard        |
| `Sales_Forecasting_Project_Report_Eyesly.pdf` | 📘 Full project report for recruiters                  |
| `dashboard_visuals/`                          | Screenshots of each Power BI page (JPG/PNG format)     |
| `README.md`                                   | This file — full project overview                      |
| `.gitignore`                                  | Ignoring temp, logs, checkpoints                       |
| `LICENSE`                                     | MIT License                                            |

---

## 🛠️ Tools Used

- **Python** — pandas, scikit-learn, statsmodels
- **Power BI** — dashboard visualizations
- **Git & GitHub** — version control & collaboration

---

## 📘 Project Report

A complete project report is included:
📄 [Download Report (PDF)](Sales_Forecasting_Project_Report_Eyesly.pdf)

Covers:
- Data exploration
- Feature engineering
- Time series modeling
- ML insights
- Power BI dashboard explanation

---

## 📊 Project Presentation

Explore the complete presentation of this project here:  
👉 [Sales Forecasting for Retail using ARIMA, ETS, and Random Forest](https://gamma.app/docs/Sales-Forecasting-for-Retail-using-ARIMA-ETS-and-Random-Forest-en841ffzrm5g4dm)

------------

## 👩‍💻 Author

**Eyesly Meribha Johnson Paulraj**  
Data Scientist | MSc Data Science | Python, Power BI, Time Series  
📎 [LinkedIn](https://www.linkedin.com/in/eyesly-meribha-johnson-paulraj-7a8b49221)  
📂 [Power BI Dashboard Folder](https://drive.google.com/drive/u/0/folders/1SA_Tl1PJRE7xYKICO3M07leajcOfvjiT)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 💼 For Recruiters & Hiring Managers

This project showcases:
- Complete ML pipeline implementation
- Business-oriented dashboard storytelling
- Real-world forecasting problem-solving
- End-to-end documentation & GitHub portfolio readiness

Please feel free to explore the notebook, dashboard, and report. Feedback is welcome!
