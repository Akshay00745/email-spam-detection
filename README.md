# 📧 Email Spam Detection using Machine Learning

## 📌 Project Overview
This project focuses on building a machine learning system to classify emails as
**Spam** or **Ham (Not Spam)** based on their textual content.

Email spam detection is a classic and widely deployed NLP use case, essential for
protecting users from phishing, scams, and unwanted messages.

---

## 📊 Dataset Description
The dataset consists of email messages with the following columns:

- `text`      → Email content
- `label`     → spam / ham
- `label_num` → Binary target (1 = spam, 0 = ham)

The dataset shows a natural class imbalance, reflecting real-world email traffic.

---

## 🔍 Exploratory Data Analysis (EDA)

### Key Analyses Performed:
- Spam vs Ham distribution
- Message length comparison
- Most frequent words in spam messages

### EDA Insights:
- Ham messages are more frequent than spam
- Spam messages tend to be longer on average
- Spam messages contain promotional and urgency-based words
  such as “free”, “call”, “win”, and “offer”

---

## 🧹 Text Preprocessing
Steps applied to clean the text data:
- Converted text to lowercase
- Removed special characters and numbers
- Removed stopwords
- Applied stemming
- Created cleaned text for modeling

---

## 🔠 Feature Engineering
- TF-IDF Vectorization used to convert text into numerical features
- Limited to top features to avoid overfitting

---

## 🤖 Models Trained

### 1. Naive Bayes
- Well-suited for text classification
- Fast and effective baseline model

### 2. Logistic Regression
- Strong linear classifier
- Performs well with TF-IDF features

---

## 📊 Model Evaluation

### Naive Bayes Performance:
- Accuracy: ~95%
- Spam Recall: ~96%
- Spam Precision: ~88%

### Logistic Regression Performance:
- Accuracy: ~98%
- Spam Recall: ~97%
- Spam Precision: ~96%

### Key Takeaway:
Both models performed exceptionally well, with **Logistic Regression achieving the
best overall balance between precision and recall**, making it the final choice.

---

## 🧠 Key Learnings
- Accuracy alone is not sufficient; precision and recall matter in spam detection
- TF-IDF + simple models can outperform complex approaches
- Logistic Regression provides strong, interpretable performance

---

## 📁 Project Structure
