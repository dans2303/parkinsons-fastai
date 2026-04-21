# 🧠 Parkinson’s Disease Detection using Deep Learning (FastAI) and Model Comparison

## 📌 Overview

This project explores **deep learning for Parkinson’s disease detection** using voice-based biomedical features and compares it with classical machine learning approaches.

It is a continuation of a machine learning pipeline developed using:

- Gradient Boosting
- XGBoost

👉 This repository focuses on:

- FastAI Tabular (Deep Learning)
- Comparative analysis between machine learning and deep learning models

---

## 🧬 Problem Background

Parkinson’s disease is a progressive neurological disorder that affects motor control and speech.

Research shows that subtle voice variations — such as jitter, shimmer, and noise-related features — can serve as early biomarkers.

This project leverages these features to enable **non-invasive and cost-effective disease detection**.

---

## 🤖 Deep Learning Approach

This repository implements a **FastAI Tabular model** for structured biomedical data.

Key components include:

- Multi-layer neural network architecture  
- Feature normalization  
- Class imbalance handling using weighted loss  
- Threshold tuning for improved medical relevance  

---

## ⚙️ Experimental Setup

To ensure fair comparison across models:

- Same dataset and feature set are used  
- Stratified 80/20 train-test split  
- Evaluation metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - ROC-AUC
  - MCC (Matthews Correlation Coefficient)

---

## 📊 Model Comparison

This study compares three approaches:

| Model | Type |
|------|------|
| Gradient Boosting | Classical ML |
| XGBoost | Advanced ML |
| FastAI Tabular | Deep Learning |

---

## 📈 Results

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC | MCC |
|------|--------|--------|--------|--------|--------|--------|
| Gradient Boosting | 0.9565 | 0.9737 | 0.9737 | 0.9737 | 0.9868 | 0.8487 |
| XGBoost | 0.9348 | 0.9268 | **1.0000** | 0.9620 | 0.9638 | 0.7611 |
| FastAI Tabular | **0.9565** | 0.9737 | 0.9737 | 0.9737 | **0.9901** | **0.8487** |

---

## 🔍 Key Insights

- **FastAI Tabular** achieved the best overall performance (highest ROC-AUC)  
- **Gradient Boosting** produced the most balanced predictions  
- **XGBoost** achieved perfect recall, meaning no Parkinson cases were missed  

---

## 🧠 Interpretation

- Deep learning improves **class separation** (higher ROC-AUC)  
- Classical machine learning remains highly competitive on tabular data  
- Boosting models are particularly effective for **recall-critical applications**  

👉 Model selection should be guided by application goals:
- Screening → maximize recall  
- Diagnosis → balanced performance  
- General prediction → overall performance  

---

## 🏥 Practical Implications

- **Screening systems** → XGBoost (no missed patients)  
- **Balanced diagnostic tools** → Gradient Boosting  
- **General predictive systems** → FastAI Tabular  

---

## 📁 Project Structure

```text
parkinsons-fastai/
│
├── models/
│   └── final_model_comparison.csv
│
├── notebooks/
│   ├── fastai_tabular_parkinsons.ipynb
│   └── 02_model_comparison_parkinsons.ipynb
│
└── README.md

---

## 🔗 Related Work

👉 Machine Learning pipeline:  
`parkinsons-xgboost`

This includes:
- full preprocessing pipeline  
- feature engineering  
- SMOTETomek balancing  
- Gradient Boosting and XGBoost models  

---

## 🚀 Future Work

- Cross-validation for more robust evaluation  
- CNN-based spectrogram models  
- Real-time inference system  
- Integration with FastAPI  

---

## 📬 Contact

- 📧 Email: mirnadanisat@gmail.com  
- 🔗 LinkedIn: https://www.linkedin.com/in/mirnadanisatandjung/

---

## ⭐ Final Note

This project demonstrates that both **machine learning and deep learning** can effectively detect Parkinson’s disease from structured voice features.

The key takeaway is that **model performance must be interpreted in context**, not judged by a single metric such as accuracy.
