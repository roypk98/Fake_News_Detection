# 📰 Fake News Detection Using Word2Vec

## 👥 Team Members
- **Piyush Kumar Roy**  
- **Anu Thomas**

---

## 🎯 Objective

The goal of this project is to develop a **Semantic Classification model** that leverages **Word2Vec** to classify news articles as either *True* or *Fake*. The focus is on capturing the **semantic meaning** behind text rather than relying solely on syntax, building a system capable of identifying misinformation effectively.

---

## 🧠 Business Motivation

The digital age has accelerated the spread of news through various online platforms. Unfortunately, it has also made it easier for *fake news* to proliferate. The consequences of such misinformation can be severe, affecting public trust and societal stability. This project aims to combat that by building a system that:

- Automatically classifies news articles as **True** or **Fake**
- Reduces the spread of **misleading information**
- Supports **fact-based journalism** and **public awareness**

---

## 🛠️ Technologies Used

```bash
# Install required packages
!pip install --upgrade numpy==1.26.4
!pip install --upgrade pandas==2.2.2
!pip install --upgrade nltk==3.9.1
!pip install --upgrade spacy==3.7.5
!pip install --upgrade scipy==1.9.3
!pip install --upgrade pydantic==2.10.5
!pip install wordcloud==1.9.4

# Download spaCy English language model
!python -m spacy download en_core_web_sm
```

---

## 🗂️ Dataset Information

You will be working with two CSV files:

- **True.csv** — 21,417 real news articles  
- **Fake.csv** — 23,502 fake news articles  

Each file contains the following columns:

- `title` — The headline of the news article  
- `text` — The body/content of the article  
- `date` — Publication date  

---

## 🔄 Project Pipeline

Below are the sequential tasks performed to build the Fake News Detection model:

### 1. Data Preparation
- Load and merge True and Fake datasets
- Assign appropriate labels (`1` for true, `0` for fake)

### 2. Text Preprocessing
- Tokenization
- Lemmatization
- Stop word removal
- Lowercasing and punctuation removal

### 3. Exploratory Data Analysis (EDA)
- Perform EDA on Training Data
- Optional: Perform EDA on Validation Data
- Visualizations (WordClouds, frequency plots)

### 4. Train-Validation Split
- Split dataset into training and validation sets

### 5. Feature Extraction
- Convert text to vector representation using **Word2Vec**
- Aggregate word vectors for sentence-level embeddings

### 6. Model Training and Evaluation
- Train supervised classifiers (e.g., Logistic Regression, SVM)
- Evaluate using metrics such as:
  - Accuracy
  - Precision
  - Recall
  - F1 Score

---

## 📌 Final Notes

This assignment helps develop an understanding of how **semantic relationships** between words can be used in **text classification**. With techniques like Word2Vec, the model doesn't just look at surface-level patterns but also captures the contextual meaning of news content—crucial in distinguishing fake from true news in real-world applications.
