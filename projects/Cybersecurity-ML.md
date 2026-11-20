# Cybersecurity Machine Learning & Intrusion Detection

**GitHub Repository:** `kassiis/cybersecurity-ml`  
**Source code:** Private repository  
**Project Category:** Machine Learning & Cybersecurity  
**Development Status:** Completed Practical Work & Benchmark Study  

---

## 1. Overview

**Cybersecurity Machine Learning** is an empirical research and practical implementation suite evaluating machine learning models for cybersecurity applications, with a primary focus on network intrusion detection systems (NIDS) and comparative algorithm performance across high-dimensional benchmark datasets.

---

## 2. Project Purpose

Modern enterprise networks generate massive volumes of telemetry where static signature-based detection mechanisms fail against novel attack vectors. This project explores:

- The effectiveness of supervised learning classifiers in identifying malicious network behaviors.
- The separation characteristics of unsupervised clustering algorithms when applied to high-dimensional network telemetry.
- Empirical benchmarking of ensemble methods versus single-estimator models under imbalanced class distributions.

---

## 3. Key Capabilities & Methodologies

- **Intrusion Detection Modeling:** Preprocessing, feature encoding, scaling, and evaluation using the modern **UNSW-NB15** cybersecurity benchmark dataset.
- **Ensemble Classifier Evaluation:** Comparative training and benchmarking of ensemble algorithms including Random Forest, AdaBoost, and Gradient Boosting against base decision trees.
- **Multi-Algorithm Benchmarking:** Rigorous baseline comparisons across diverse model families:
  - Support Vector Machines (SVM)
  - K-Nearest Neighbors (KNN)
  - Gaussian Naive Bayes
  - Regularized Logistic Regression
- **Comprehensive Performance Diagnostics:** Evaluation across rigorous diagnostic metrics including Accuracy, Precision, Recall, F1-Score, Confusion Matrices, ROC-AUC curves, and Stratified K-Fold Cross-Validation.
- **Unsupervised Clustering Studies:** Comparative analysis of dimensional reduction and data clustering structures to analyze natural groupings and anomaly separation.

---

## 4. Technologies Used

- **Language:** Python 3
- **Data Manipulation & Analysis:** NumPy, pandas
- **Machine Learning & Modeling:** scikit-learn
- **Visualization & Diagnostics:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebooks, Python CLI Scripts

---

[← Return to Project Portfolio](../README.md)
