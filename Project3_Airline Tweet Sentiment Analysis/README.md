✈️ Airline Tweet Sentiment Analysis using NLP and Streamlit
A full-stack NLP project that classifies customer sentiment in airline-related tweets using machine learning and natural language processing, deployed via an interactive Streamlit app. Includes detailed EDA, text cleaning, model evaluation, and multi-page visualizations for insights.
------------------------
📊 Business Problem
Airlines receive thousands of customer tweets daily, covering feedback on service quality, flight delays, baggage handling, and overall experience. Manual review is time-consuming and inconsistent.

This project automates sentiment classification to help:

Improve customer experience

Identify recurring issues

Assist marketing & service teams with real-time sentiment analysis

---------------------------------

📁 Dataset Overview
This project uses the Twitter US Airline Sentiment dataset from Kaggle, including:

airline – Airline mentioned in the tweet

airline_sentiment – Sentiment label (positive, neutral, negative)

text – Raw tweet text

negativereason – Reason for negative feedback (if applicable)

Final features after preprocessing:

clean_text – Cleaned, lemmatized version of tweet

label – Encoded sentiment label (0 = Negative, 1 = Neutral, 2 = Positive)
=======================

🔍 Methodology
1. Text Preprocessing
Removed links, mentions, punctuation, numbers

Lowercased, tokenized, stopword removed

Lemmatization using WordNetLemmatizer

2. Feature Extraction
TF-IDF Vectorizer (max_features=5000, bigrams included)

3. Model Training
Model: Multinomial Naive Bayes

Dataset split: train_test_split (80/20)

4. Evaluation
Accuracy: ✅ 0.74

Confusion Matrix

Classification Report with Precision, Recall, F1-Score

=======================================

📈 Visual Analysis Dashboard
All visuals are stored in the GitHub repo under visualizations/. These represent insights designed for stakeholder review.

Page	Description
1	✅ Model Accuracy, 📊 Classification Report, 🧮 Confusion Matrix
2	Per-airline evaluation: accuracy & confusion matrix by airline
3	📉 Confusion Matrix Heatmap
4	📊 Sentiment Distribution by Airline
5	🔺 Top Reasons for Negative Sentiment + 📈 Sentiment Trends Over Time


======================================

📦 Repository Contents
File / Folder	Purpose
notebooks/01_sentiment_analysis_airlines.ipynb	Jupyter notebook (EDA, modeling, evaluation)
data/Tweets.csv	Original dataset from Kaggle
models/sentiment_model.pkl	Trained Naive Bayes classifier
models/tfidf_vectorizer.pkl	Trained TF-IDF vectorizer
app/streamlit_app.py	Streamlit app for real-time sentiment prediction
visualizations/	Sentiment plots & confusion matrix heatmaps
requirements.txt	Environment dependencies
README.md	Project documentation (this file)
.gitignore	Ignored files (e.g., checkpoints, models)

========================

🖥️ Streamlit App
An interactive app where users can enter any tweet and get a real-time sentiment prediction using the trained model.

=====================================
🛠 Run Locally:
bash

pip install -r requirements.txt
streamlit run app/streamlit_app.py

============================================

📊 Key Results
✅ Accuracy: 74%
Sentiment	Precision	Recall	F1-score	Support
Negative	0.73	0.97	0.84	1835
Neutral	0.70	0.29	0.41	620
Positive	0.86	0.42	0.56	473

Model handles negative tweets well, but performance can improve for neutral/positive classes

Top 10 reasons for negative sentiment include: customer service, flight late, baggage, etc.

==============================

🧠 Sample Visuals
🔹 Sentiment Distribution by Airline

🔹 Top Reasons for Negative Sentiment

🔹 Sentiment Trend Over Time

=======================================================

🛠 Tools Used
Python: pandas, nltk, scikit-learn, matplotlib, seaborn

NLP: Stopword removal, Lemmatization, TF-IDF

Model: Multinomial Naive Bayes

App: Streamlit

Version Control: Git & GitHub


=====================

📘 Project Report
Jupyter Notebook:
📂 notebooks/01_sentiment_analysis_airlines.ipynb

Includes:

Data loading

EDA

Preprocessing

Modeling

Evaluation

Visualizations


====================


👩‍💻 Author
Eyesly Meribha Johnson Paulraj
Data Scientist | MSc Data Science
📌 Python | 🧠 NLP | 🚀 Streamlit | 📊 Machine Learning

🔗 LinkedIn

======================

📄 License
This project is licensed under the MIT License.


==========================

💼 For Recruiters & Hiring Managers
This project showcases:

A full NLP pipeline implementation

Real-world social media sentiment classification

Streamlit-based model deployment

Insightful visualizations for decision-makers

GitHub-ready, clean documentation & reporting

🔍 Feel free to explore the notebook, app, and visuals. Feedback is welcome!
