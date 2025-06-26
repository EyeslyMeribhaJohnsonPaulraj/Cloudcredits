# 🛡️ Credit Card Fraud Detection with Random Forest & SHAP
An end-to-end data science project that applies machine learning techniques to detect fraudulent credit card transactions. The project includes preprocessing imbalanced data, model training, evaluation with recall-focused metrics, and a reporting dashboard.

---

📊 **Business Problem**

Credit card fraud causes major losses for financial institutions and customers. Detecting fraud early helps prevent unauthorized access and financial crimes.  
This project builds a classification model that flags potentially fraudulent transactions using historical, anonymized credit card data.

**Goals:**
- Maximize fraud detection recall
- Minimize false negatives
- Provide explainable AI outputs to support fraud analysts

---

📁 **Dataset Overview**

This project uses anonymized transaction data from Kaggle:

- 284,807 credit card transactions
- 492 fraudulent transactions (~0.17%)
- Features: 28 anonymized PCA components, `Time`, `Amount`, and `Class` (target)
  
**Data Source:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

🔍 **Methodology**

1. **Exploratory Data Analysis (EDA)**
   - Visualize class imbalance
   - Analyze `Amount`, `Time`, and distribution across fraud vs. non-fraud

2. **Data Preprocessing**
   - No missing values
   - Scaled `Amount` feature
   - Handled class imbalance using class weights

3. **Modeling**
   - Algorithm: `RandomForestClassifier`
   - Evaluation metrics: Precision, Recall, F1-Score, ROC-AUC
   - Focus on **high recall** to catch more frauds

4. **Explainability (SHAP)**
   - SHAP used to interpret key features contributing to fraud detection
   - Summary plots provided in the outputs folder

---

📈 **Streamlit App**

A web-based tool using [Streamlit](https://streamlit.io/) to:

- Upload and inspect new transaction files
- Display class distribution
- Preview suspicious patterns

Run it using:
```bash
cd streamlit_app
streamlit run streamlit_app.py
📸 Dashboard Visuals


=====================

## Tableau-style dashboard includes:

Page	Description
1	Dataset Overview & Fraud Distribution
2	Transactions by Time & Amount
3	Model Evaluation Results (Confusion Matrix, ROC Curve)
4	SHAP Feature Importance (Explainable AI)
5	Final Insights for Business Use

Visuals are provided in the dashboard/ folder as PDF format. You may replace it with .twbx if using Tableau.

========================
##📦 Repository Contents

File	Purpose
📓 Fraud_Detection_Complete.ipynb	Full notebook: EDA → Model → Evaluation
📄 confusion_matrix.csv	Confusion matrix output
📄 shap_summary_plot.png	SHAP plot for feature interpretation
📂 dashboard/Fraud_Detection.pdf	Fraud insights visualized
📁 streamlit_app/streamlit_app.py	Streamlit web app
📁 reports/summary_report.md	Key results and SHAP summary
📁 data/creditcard.csv	📌 Placeholder — replace with real Kaggle file
📄 requirements.txt	Python libraries required
📄 README.md	This file — full project overview
📄 LICENSE	MIT License

====


### 🛠️ Tools Used

Python — pandas, scikit-learn, seaborn, matplotlib, shap

Streamlit — Interactive fraud visualization

Tableau — Dashboard (PDF/PNG provided)

Git & GitHub — Version control and collaboration
-------------------------

📘 Project Report

A concise project report is available in reports/summary_report.md (or PDF if exported):

Problem understanding

EDA highlights

Model strategy and evaluation

SHAP explainability notes

Dashboard walkthrough



========================


👩‍💻 Author

Eyesly Meribha Johnson Paulraj
Data Scientist | MSc Data Science | Python, Machine Learning, Power BI
📎 linkedin.com/in/eyesly-meribha-johnson-paulraj-7a8b49221


===================================

📄 License

This project is licensed under the MIT License.
You are free to use, share, and modify with appropriate attribution.


=====================================

💼 For Recruiters & Hiring Managers

This project showcases:

Real-world fraud detection use case

Class imbalance handling with business focus

Explainable AI using SHAP

Streamlit app + Dashboard storytelling

GitHub documentation & full pipeline structure

Please explore the notebook, dashboard, and Streamlit app. Feedback is welcome!
