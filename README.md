# 🗣️ Voice to Verdict: Truth/Lie Detection with Machine Learning

This repository contains a mini-project submitted for the **ECS7020P – Principles of Machine Learning** module at **Queen Mary University of London**. The objective is to detect **truthful vs. deceptive statements** using supervised machine learning on linguistic features derived from audio transcripts.

---
## 📊 Dataset Details

- **File:** `MLEndDeception_small.csv`
- **Size:** Small subset of larger deceptive speech corpus
- **Features:** Raw text + labels (`truthful`, `deceptive`)
---

## ✅ What Did I Build?

I developed a binary classification system that analyzes text derived from speech and predicts whether a statement is **truthful** or **deceptive**. The model was trained on labeled samples and deployed in a Jupyter Notebook using scikit-learn pipelines.

---

## ⚙️ How Does It Work?

- **Dataset**: `MLEndDeception_small.csv` with labeled samples of true/false statements.
- **Preprocessing**:
  - Cleaned and tokenized text
  - Removed stopwords and punctuations
  - Extracted features using TF-IDF and semantic tags
- **Model Training**:
  - Tested multiple classifiers: Logistic Regression, SVM, Random Forest
  - Tuned hyperparameters using cross-validation
  - Evaluated using precision, recall, F1-score
- **Visualization**:
  - Word clouds
  - Label distributions
  - Confusion matrix


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
## 📚 Key Learnings

- **Text preprocessing choices matter** — lemmatization, stopwords, and token length affect model performance
- **TF-IDF outperformed simpler frequency-based vectors**, especially with Logistic Regression
- **SVMs excelled in high-dimensional sparse spaces** like TF-IDF
- **Model explainability** (through confusion matrix and feature weights) is vital when dealing with sensitive classifications
- **Semantic enrichment** (POS tags, sentence structure) can improve performance but adds computational complexity

---

## 🚀 How to Run

1. Clone the repository  
   git clone https://github.com/YOUR_USERNAME/ml-end-deception.git
   cd ml-end-deception```

2. Install the dependencies
```pip install -r requirements.txt```

3. Launch the notebook
```jupyter notebook ECS7020P_miniproject_submission.ipynb```
