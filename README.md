# 🧠 Parkinson’s Disease Detection using Deep Learning (FastAI) and Model Comparison

## 📌 Overview

This project explores **deep learning for Parkinson’s disease detection** using voice-based biomedical features and compares it with classical machine learning approaches.

It builds upon a prior machine learning pipeline developed using:

- Gradient Boosting
- XGBoost

This repository focuses on:

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

### Key Components

- Multi-layer neural network architecture
- Feature normalization
- Class imbalance handling using weighted loss
- Threshold tuning for improved medical relevance

---

## ⚙️ Experimental Setup

To ensure fair comparison across models:

- Same dataset and feature set are used
- Stratified 80/20 train-test split

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- MCC (Matthews Correlation Coefficient)

---

## 📊 Model Comparison

| Model | Type |
|------|------|
| Gradient Boosting | Classical ML |
| XGBoost | Advanced ML |
| FastAI Tabular | Deep Learning |

---

## 📈 Results

### Performance Comparison

| Model | Accuracy | Recall | ROC-AUC | MCC |
|:------|:--------:|:------:|:------:|:----:|
| Gradient Boosting | 0.9565 | 0.9737 | 0.9868 | 0.8487 |
| XGBoost | 0.9348 | **1.0000** | 0.9638 | 0.7611 |
| FastAI Tabular | **0.9565** | 0.9737 | **0.9901** | **0.8487** |

### Key Insights

- **FastAI Tabular** → best overall performance (highest ROC-AUC)
- **Gradient Boosting** → most balanced predictions
- **XGBoost** → perfect recall (no missed cases)

---

## 🧠 Interpretation

- Deep learning improves **class separation**
- Classical ML remains highly competitive for tabular data
- Boosting models are strong for **recall-critical applications**

Model selection should depend on application goals:

- Screening → maximize recall
- Diagnosis → balanced performance
- General prediction → overall performance

---

## 🏥 Practical Implications

- **Screening systems** → XGBoost
- **Balanced diagnostic tools** → Gradient Boosting
- **General predictive systems** → FastAI Tabular

---

## 📁 Project Structure

```text
parkinsons-fastai/
├── models/
│   └── final_model_comparison.csv
├── notebooks/
│   ├── 01_fastai_tabular_parkinsons.ipynb
│   └── 02_model_comparison_parkinsons.ipynb
└── README.md
```

---

## 🔗 Related Work

Machine Learning pipeline: parkinsons-xgboost

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

📧 Email: mirnadanisat@gmail.com

🔗 LinkedIn: https://www.linkedin.com/in/mirnadanisatandjung/
