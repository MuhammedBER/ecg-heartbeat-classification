<h1 align="center">🫀 ECG Heartbeat Classification</h1>
<p align="center">
  A comparative study of machine learning and deep learning models for ECG heartbeat classification.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat&logo=python&logoColor=white"/>
</p>

---

## 📌 Overview

This project compares four machine learning and deep learning models for classifying ECG heartbeats into 5 categories. The goal is both to benchmark model performance and to identify the best candidate for real-world cardiac monitoring applications.

---

## 🏷️ Classes

| Class | Description |
|---|---|
| N | Normal |
| S | Supraventricular |
| V | Ventricular |
| F | Fusion |
| Q | Unknown |

---

## 🏆 Model Comparison

### Overall Performance

| Model | Accuracy | Macro F1 |
|---|---|---|
| Logistic Regression | 67.44% | 0.4789 |
| SVM | 95.57% | 0.8094 |
| Random Forest | **97.23%** | **0.8521** |
| CNN | 97.06% | 0.8614 |

### Per Class F1 Score

| Class | Logistic Reg | SVM | Random Forest | CNN |
|---|---|---|---|---|
| Normal | 0.78 | 0.98 | 0.98 | 0.98 |
| Supraventricular | 0.24 | 0.62 | 0.75 | 0.74 |
| Ventricular | 0.42 | 0.93 | 0.93 | 0.91 |
| Fusion | 0.15 | 0.55 | 0.63 | 0.69 |
| Unknown | 0.81 | 0.98 | 0.97 | 0.97 |

---

## 🔍 Key Findings

- **Random Forest** achieved the highest overall accuracy at **97.23%**
- **CNN** achieved the best Macro F1 at **0.8614**, making it the most balanced model across all classes
- **Logistic Regression** struggled significantly with minority classes (Supraventricular, Fusion)
- **SVM and Random Forest** are strong classical ML baselines for this task
- For real-world use, **CNN is recommended** due to its balanced performance across all heartbeat types

---

## 📦 Dataset

**Segmented and Preprocessed ECG Signals for Heartbeat Classification**
Available on Kaggle: [ECG Heartbeat Categorization Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat)

---

## 🛠️ Tech Stack

| Tool | Usage |
|---|---|
| TensorFlow / Keras | CNN model |
| scikit-learn | Logistic Regression, SVM, Random Forest |
| Pandas | Data loading & preprocessing |
| Matplotlib | Visualization & results plotting |

---

## 🚀 Getting Started

### Prerequisites
```bash
pip install tensorflow scikit-learn pandas matplotlib
```

### Run
Open the notebook:
```bash
jupyter notebook ecg_classification.ipynb
```

---

## 👨‍💻 Author

**Mohamed Berhaila**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/mohamed-berhaila)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white)](https://berhaila.com)