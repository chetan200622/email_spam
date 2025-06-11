# email_spam
# 📧 Email Spam Classifier using Machine Learning

This project implements an intelligent email spam classifier using machine learning. It analyzes email content and classifies it as **spam** or **ham** (not spam) using a Logistic Regression model trained on a labeled dataset.

---

## 🚀 Project Overview

Spam emails often contain misleading content like fake offers, suspicious links, and clickbait subject lines. The goal of this project is to build a system that can automatically detect and filter out such spam messages to protect users and enhance email usability.

---

## 🧠 Model Used

- **Machine Learning Algorithm**: Logistic Regression
- **Feature Extraction**: TF-IDF Vectorizer (Term Frequency–Inverse Document Frequency)
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1 Score

---

## 🧰 Technologies & Libraries

- Python 3.13.1
- pandas
- NumPy
- scikit-learn

---

## 📁 Dataset

- **File**: `mail_data.csv`
- **Columns**:
  - `Category`: Label (`spam` or `ham`)
  - `Message`: The actual email text

---

## ⚙️ How It Works

1. **Data Preprocessing**
   - Handle missing values
   - Encode target labels (`spam` = 0, `ham` = 1)
   - Clean and normalize text data

2. **Feature Extraction**
   - Use `TfidfVectorizer` to convert messages into numerical features

3. **Model Training**
   - Split the data into training and test sets
   - Train a `LogisticRegression` model using the training data

4. **Model Evaluation**
   - Predict on test data and compute accuracy
   - Example accuracy: ~96% on test set

5. **Prediction**
   - Take a new input message and classify it as spam or ham

---

## 🔍 Sample Output

```python
Input: "SIX chances to win CASH! From 100 to 20,000 pounds..."
Prediction: Spam mail
