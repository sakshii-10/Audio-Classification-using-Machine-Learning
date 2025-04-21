# Audio-Classification-using-Machine-Learning
A machine learning-based deception detection project for ECS7020P (Principles of Machine Learning) at Queen Mary University of London. This project explores various classifiers and semantic feature engineering techniques to identify truthful vs deceptive statements.


# 🤖 Deception Detection using Machine Learning

This repository contains a mini-project submitted for the **ECS7020P – Data Semantics** module at **Queen Mary University of London**. The goal of the project is to classify **truthful vs deceptive statements** using traditional and semantic-aware machine learning techniques.

---

## 📊 Dataset

- **File:** `MLEndDeception_small.csv`
- Contains labeled samples of truthful and deceptive text-based statements.
- Preprocessed with tokenization, vectorization, and possibly semantic features (e.g., POS tags, TF-IDF).

---

## 🧠 Approach

- **Exploratory Data Analysis**: Label distribution, text lengths, word clouds.
- **Preprocessing**: Tokenization, TF-IDF vectorization, stopword removal.
- **Models Used**:
  - Logistic Regression
  - SVM (Linear/Kernel)
  - Random Forest / Decision Trees
  - (Optional) Word Embeddings or NLP semantic features
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## 🚀 How to Run

1. Clone the repository  
   git clone https://github.com/YOUR_USERNAME/ml-end-deception.git
   cd ml-end-deception```

2. Install the dependencies
```pip install -r requirements.txt```

3. Launch the notebook
```jupyter notebook ECS7020P_miniproject_submission.ipynb```
