# Airline Sentiment Analysis using NLP & Machine Learning

A full-stack Natural Language Processing (NLP) project that classifies airline-related tweets into sentiment categories (Positive, Neutral, Negative) and extracts business insights using Machine Learning.

---

## Business Problem

Airlines receive thousands of social media messages daily, making it difficult to manually analyze customer sentiment. This project builds a sentiment classification system that helps identify:

- Overall brand sentiment
- Frequent negative feedback categories
- Trends in customer satisfaction over time

---

## 📁 Dataset Overview

**Source:** [Kaggle – Twitter US Airline Sentiment](https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment)

| Column             | Description                                 |
|--------------------|---------------------------------------------|
| `text`             | Raw tweet content                           |
| `airline`          | Airline name                                |
| `airline_sentiment`| Sentiment (positive, neutral, negative)     |
| `negativereason`   | Reason for negative feedback (if applicable)|

---

## Methodology

1. **Text Cleaning & Preprocessing**
   - Removed mentions, hashtags, punctuation, digits
   - Tokenization, stopword removal, lemmatization

2. **Feature Engineering**
   - TF-IDF vectorization (bi-grams, 5000 features)

3. **Modeling**
   - Algorithm: Multinomial Naive Bayes
   - Accuracy: **74.04%**

4. **Evaluation Metrics**
   - Confusion Matrix
   - Precision, Recall, F1-Score
   - Classification Report

---

## 📈 Visual Insights

| Page | Description |
|------|-------------|
| 1️⃣   | Accuracy, Confusion Matrix, Classification Report |
| 2️⃣   | Sentiment Distribution by Airline |
| 3️⃣   | Top 10 Reasons for Negative Sentiment |
| 4️⃣   | Sentiment Trends Over Time (Simulated) |
| 5️⃣   | Streamlit-based Sentiment Classifier UI |

---

## Web App (Streamlit)

A live classifier built with **Streamlit** that predicts the sentiment of user-input airline tweets.

**Demo Interface:**

```bash
streamlit run streamlit_app.py
🧰 Tools & Technologies
Python (Pandas, NumPy, Scikit-learn, NLTK)

Matplotlib, Seaborn

Streamlit (for deployment)

Git & GitHub

--------------------------

📦 Repository Structure


Airline-Sentiment-Analysis/
│
├── sentiment_analysis_notebook.ipynb     # Full project code
├── streamlit_app.py                      # Streamlit deployment
├── sentiment_model.pkl                   # Trained sentiment classifier
├── tfidf_vectorizer.pkl                  # Saved TF-IDF vectorizer
├── requirements.txt                      # Python dependencies
├── LICENSE                               # MIT License
├── .gitignore                            # Ignored system files
├── visuals/                              # Images used in README/report
│   ├── confusion_matrix.png
│   ├── sentiment_by_airline.png
│   ├── top_negative_reasons.png
│   └── sentiment_trends.png
│
├── Airline_Sentiment_Report_Eyesly.pdf   # 📘 Full project report
└── README.md                             

=======================

📘 Project Report & Presentation
📄 Download Full Report (PDF)

🎞️ Presentation (PPTX)

Explore the complete presentation of this project here:  
👉 [Airline Sentiment Analysis using NLP & Machine Learning] (https://gamma.app/docs/Airline-Sentiment-Analysis-using-NLP-Machine-Learning-gs99nc7kj2gmhfx)
 
===========

👩‍💻 Author
Eyesly Meribha Johnson Paulraj
Data Scientist | MSc Data Science
linkedin.com/in/eyesly-meribha-johnson-paulraj-7a8b49221

======================================

📄 License
This project is licensed under the MIT License – see the LICENSE file for details.

=======================

💼 For Recruiters & Hiring Managers
This project showcases:

A complete machine learning pipeline
Real-world text data analysis
Business-driven insights
Deployment-ready code
Clean documentation and GitHub portfolio structure
