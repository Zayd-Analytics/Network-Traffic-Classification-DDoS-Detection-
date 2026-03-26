# Network Traffic Classification — DDoS Detection

## Overview
A machine learning system to classify network traffic flows
as normal or attack categories. Built to improve intrusion
detection accuracy, reduce false positives, and enhance
overall network security posture.

Built as part of the BIA® Research Internship at
First Quadrant Labs. Project 2 of 6.

## Problem Statement
Traditional rule-based intrusion detection systems struggle
with sophisticated DDoS attacks and generate high false
positive rates. This project uses flow-based ML classification
to automate and improve detection accuracy.

## Dataset
- **Type:** Network flow features
- **Task:** Multi-class classification
- **Target:** Normal traffic vs attack categories
- **Challenge:** Class imbalance between normal and attack traffic

## Methodology
1. Data Loading & Inspection
2. Data Preprocessing & Class Imbalance Handling
3. Exploratory Data Analysis — attack pattern visualization
4. Feature Selection — identifying top intrusion indicators
5. Model Training — Logistic Regression, Random Forest, SVM
6. Ensemble Evaluation & Cross-Validation
7. ROC-AUC Analysis & Leakage Checks
8. Final Model Selection & Business Recommendations

## Model Results
| Model | Notes |
|---|---|
| Logistic Regression | Baseline — linear decision boundary |
| SVM | Strong on high-dimensional flow features |
| **Random Forest** | **Best performer — selected as final model** |

**Evaluation:** Stratified cross-validation, ROC-AUC,
accuracy, precision, recall, F1-score

**Leakage check:** Passed — no data leakage detected

## Key Findings
- Tree-based models significantly outperform linear
  classifiers for network traffic classification
- Packet size, duration, and byte ratio features are
  the strongest attack indicators
- Class imbalance handling is critical — without it,
  minority attack classes are consistently misclassified
- Stratified cross-validation essential for reliable
  performance estimates on imbalanced datasets

## Tech Stack
Python • Scikit-learn • Pandas • NumPy •
Matplotlib • Seaborn • Jupyter Notebooks

## Deliverables
- `notebook.ipynb` — Full classification pipeline
- `presentation.pptx` — Project summary & findings

## About
Part of a 6-month BIA® Research Internship at
First Quadrant Labs.
Project 2 of 6 — cybersecurity domain.
