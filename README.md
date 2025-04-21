# 🗣️ Voice to Verdict: Truth/Lie Detection with Machine Learning

This repository contains a mini-project submitted for the **ECS7020P – Principles of Machine Learning** module at **Queen Mary University of London**. The objective is to detect **truthful vs. deceptive statements** using supervised machine learning on linguistic features derived from audio transcripts.

---
## 📊 Dataset Details

- **File:** `MLEndDeception_small.csv`
- **Features:** Raw text + labels (`truthful`, `deceptive`)
- **Format**: `.wav` audio files labeled as truthful (1) or deceptive (0)
---

## ✅ What Did I Build?

A machine learning pipeline that:
- Downloads and processes a labeled deception audio dataset
- Splits audio recordings into 30-second chunks
- Extracts features from each chunk
- Trains models to predict whether the speaker is being truthful or deceptive


---
## 🧠 Approach
- Data Download: Retrieved a labeled deception speech dataset using the mlend Python package.
- Preprocessing: Skipped the first 15 seconds of each audio file to remove silence and intros.
- Chunking: Split each audio into 30-second segments to standardize input and increase data volume.
- Labeling: Saved each chunk with its corresponding label (truthful or deceptive) in chunk_labels.csv.
- Feature Extraction & Modeling (next step): Plan to extract acoustic features (e.g., MFCCs, pitch, energy) and train classification models using scikit-learn.

---
## ⚙️ How It Works

### 🔁 Preprocessing Steps
- Skips first 15 seconds of each clip (to remove intros)
- Splits audio into 30-second chunks
- Each chunk is saved and mapped to a label
- Outputs a `chunk_labels.csv` file with mapping of chunk → label

### 🔧 Feature Extraction & Modeling *(in progress or next step)*
- You can extract features using `librosa` (MFCCs, energy, pitch, etc.)
- Models like Logistic Regression, SVM, or Random Forest can be trained on chunk-level features

--- 
## 📚 Key Learnings

- Chunking audio helps balance and expand datasets
- Preprocessing steps (e.g., skipping intros) are crucial for quality training
- librosa is powerful for extracting meaningful acoustic features
- Combining ML + Audio offers great insight into speech-based applications
 ---
## 📁 Output Files
- audio_chunks/: Folder containing all processed audio chunks
- chunk_labels.csv: Mapping of chunk file → label
---

## 🚀 How to Run

1. Clone the repository  ```cd ml-end-deception```
2. Install the dependencies
```pip install -r requirements.txt```
3. Launch the notebook
```jupyter notebook ECS7020P_miniproject_submission.ipynb```
