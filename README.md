# 🏦 Bank Note Authentication using Machine Learning

## 📌 Overview

This project implements a **binary classification system** to identify whether a banknote is **genuine or forged** using statistical and machine learning techniques. The analysis is based on image-derived features obtained from wavelet-transformed banknote images.

The project focuses on:
- Exploratory data analysis
- Feature-based classification
- Training and evaluation of classical machine learning models
- Performance comparison using standard metrics

This repository is structured to be **fully reproducible** and **GitHub-ready**, with clean scripts and relative file paths.

---

## 🎯 Objectives

- Understand feature separability between genuine and forged banknotes
- Train and compare multiple classification models
- Evaluate models using accuracy and confusion matrices
- Identify the best-performing classifier
- Present results in a clear and interpretable manner

---

## 📂 Dataset Details

The dataset is sourced from the **UCI Machine Learning Repository**.

### Variables

| Feature     | Description                                               |
|-------------|-----------------------------------------------------------|
| variance    | Variance of the wavelet-transformed image                  |
| skewness    | Skewness of the wavelet-transformed image                  |
| curtosis    | Curtosis of the wavelet-transformed image                  |
| entropy     | Entropy of the wavelet-transformed image                   |
| class       | Target variable (0 = genuine, 1 = forged)                  |

📍 Dataset path in this repository:  
data/banknote_auth.csv

markdown
Copy code

---

## 🛠 Tools & Technologies

- **Language:** R  
- **Libraries:**
  - `tidyverse`
  - `caret`
  - `ggplot2`
  - `e1071`

- **Methods:**
  - Logistic Regression
  - k-Nearest Neighbors (k-NN)
  - Support Vector Machine (SVM)
  - (Optional) Random Forest

---

## 📁 Repository Structure

```
bank note authentication/
│
├── data/
│   └── banknote_auth.csv
│
├── notebooks/
│   ├── banknote_authentication.ipynb
│   └── Source_code.ipynb
│
├── scripts/
│   └── html.py
│
├── results/
│   ├── banknote_authentication.html
│   └── banknote_authentication.pdf
│
├── LICENSE
└── README.md

```

---

## 📊 Results Summary

- The dataset shows strong feature separability between genuine and forged banknotes.
- **Support Vector Machine (RBF kernel)** achieved the highest classification accuracy.
- **Logistic Regression** provides a strong and interpretable baseline model.
- Distance-based models such as **k-Nearest Neighbors (k-NN)** are sensitive to feature scaling.
- Detailed plots and evaluation outputs are saved in the `results/` directory.

---

## 🧠 Key Insights

- Classical machine learning models perform extremely well on this dataset.
- Non-linear decision boundaries significantly improve classification performance.
- Proper preprocessing and evaluation are crucial, even for relatively clean datasets.
- The project demonstrates a complete machine learning workflow without relying on black-box pipelines.

---

## 📜 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 📌 Notes

- This project is intended for **educational and portfolio purposes**.
- Code is written to prioritize **clarity, reproducibility, and interpretability**.
- Possible future extensions include:
  - Hyperparameter tuning
  - Cross-validation strategies

---
