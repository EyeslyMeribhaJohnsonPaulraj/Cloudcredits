# Credit Card Fraud Detection

Detecting fraudulent transactions using machine learning techniques on anonymized financial data. This project demonstrates an end-to-end data science workflow including EDA, model training, evaluation, and interactive visualization.

---

## Project Objective

Build a classification model that can detect fraudulent credit card transactions. Since fraud data is extremely imbalanced (~0.17% fraud), the project emphasizes recall and class balance using advanced evaluation techniques.

---

## 📂 Folder Structure

Fraud_Detection_Project/
├── data/ # Dataset (creditcard.csv)
├── notebooks/ # Main notebook for EDA + modeling
├── outputs/ # Trained model, confusion matrix, SHAP visuals
├── streamlit_app/ # Streamlit app code
├── dashboard/ # Tableau-style dashboard or PDF/PNG
├── reports/ # Project summary & findings
├── requirements.txt # Project dependencies
└── README.md # Project overview (this file)



---

## 📊 Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 284,807 transactions
- 492 fraud cases (≈ 0.172%)
- Features are anonymized using PCA for privacy

---

##  Key Components

### 1. **EDA (Exploratory Data Analysis)**
- Class imbalance visualization
- Transaction amount vs. class analysis
- Feature correlation heatmaps

### 2. **Data Preprocessing**
- No missing values
- Class imbalance handled using SMOTE or class weights

### 3. **Modeling**
- Classifier used: RandomForestClassifier
- Metrics: Precision, Recall, F1-Score, ROC-AUC
- Focused on high recall for fraud detection

### 4. **Evaluation**
- Confusion Matrix
- ROC Curve
- Feature importance (SHAP planned)

### 5. **Dashboard**
- Fraud vs. Non-Fraud distribution
- Trend and frequency patterns
- Can be integrated into Power BI or Tableau

---

##  How to Run

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/Credit-Card-Fraud-Detection.git
   cd Credit-Card-Fraud-Detection
Add the dataset

Place creditcard.csv inside the data/ folder.

Install dependencies

## bash

pip install -r requirements.txt
Run the notebook

Open notebooks/Fraud_Detection_Complete.ipynb in Jupyter 

Launch the Streamlit app
cd streamlit_app
streamlit run streamlit_app.py

======

📈 Visuals (Included)
📊 Confusion Matrix: outputs/confusion_matrix.csv

📉 SHAP Summary Plot: outputs/shap_summary_plot.png (generate locally)

📄 Tableau PDF Dashboard: dashboard/Fraud_Detection.pdf

============

## Skills Demonstrated
Binary classification
Imbalanced data handling
Model evaluation (recall-focused)
SHAP interpretability (planned)
Streamlit dashboarding
GitHub project structuring

====

🔐 License
This project is licensed under the MIT License.

===================

👤 Author
Eyesly Meribha Johnson Paulraj
Data Scientist | Python | SQL | Power BI | Tableau
linkedin.com/in/eyesly-meribha-johnson-paulraj-7a8b49221
