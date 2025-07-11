# 📚 Kindle Review Sentiment Analysis

A sentiment analysis project using NLP techniques to classify Kindle Store product reviews as **positive** or **negative**. This project explores different text vectorization methods like **Bag of Words (BoW)**, **TF-IDF**, and **Word2Vec** to train and evaluate machine learning models.

> 🧪 This is a practice project for learning and applying NLP concepts in Python.

---

## 🔍 Project Overview

- **Goal**: Predict sentiment (positive/negative) from Amazon Kindle Store product reviews.
- **Techniques Used**:
  - Text cleaning and preprocessing
  - Feature extraction: BoW, TF-IDF, Word2Vec
  - ML models: Logistic Regression, Naive Bayes, SVM
- **Evaluation**: Accuracy, Precision, Recall, F1 Score

---

## 📁 Dataset

### 📦 Source

- Subset of the **Amazon Kindle Store** reviews dataset (1996–2014)
- Sourced from Julian McAuley's UCSD data repository: [http://jmcauley.ucsd.edu/data/amazon/](http://jmcauley.ucsd.edu/data/amazon/)

### 🧾 Description

- Total entries: 982,619
- Each reviewer has reviewed ≥5 products; each product has ≥5 reviews

| Column          | Description                                  |
|-----------------|----------------------------------------------|
| `asin`          | Product ID                                   |
| `helpful`       | Helpfulness rating (e.g., 2/3)               |
| `overall`       | Product rating (used to derive sentiment)    |
| `reviewText`    | Full text of the review                      |
| `reviewTime`    | Date of the review                           |
| `reviewerID`    | ID of the reviewer                           |
| `reviewerName`  | Name of the reviewer                         |
| `summary`       | Summary/title of the review                  |
| `unixReviewTime`| Unix timestamp of the review                 |

📌 **Sentiment Labeling**:  
- Reviews with ratings ≥ 3 → Positive  
- Reviews with ratings ≤ 2 → Negative  

---

## 🧠 Techniques Used

- **Text Preprocessing**:
  - Lowercasing, punctuation removal, stopword removal
  - Tokenization, stemming/lemmatization
- **Vectorization**:
  - Bag of Words (BoW)
  - TF-IDF
  - Word2Vec (using Gensim)
- **Model Training**:
  - Logistic Regression
  - Multinomial Naive Bayes
  - Support Vector Machines

---

## 🏗️ Project Structure

Kindle_review_sentiment_analysis/
│
├── data/ # Dataset CSV file
├── notebooks/ # Jupyter notebooks for EDA and model building
├── models/ # Saved models (if any)
├── kindle_sentiment_analysis.py # Main script for training and evaluation
└── README.md

yaml
Copy
Edit

---

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/aniruddha26/Kindle_review_sentiment_analysis.git
cd Kindle_review_sentiment_analysis
2. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Run the code
Explore the notebooks in the folder to see step-by-step implementation.

## 📈 Results
Accuracy and F1 Score are used to compare BoW, TF-IDF, and Word2Vec methods.

Early experiments show TF-IDF and SVM/Logistic Regression perform better on this dataset.

## 📌 Acknowledgements
Dataset: Amazon product data by Julian McAuley, UCSD
📄 http://jmcauley.ucsd.edu/data/amazon/

License to the data files belongs to the original authors.

## 👨‍💻 Author
Aniruddha Alkari
