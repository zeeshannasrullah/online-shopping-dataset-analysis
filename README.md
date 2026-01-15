# 🛒 Shopping Purchase Prediction (Assignment 2 – Artificial Intelligence)

## 📘 Overview
This project is part of **Assignment 2** for the **Artificial Intelligence** course.  
The objective is to build a machine learning model that predicts whether an online shopping customer will complete a purchase based on their browsing behavior.

A **K-Nearest Neighbor (KNN)** classifier is used to classify users as buyers or non-buyers.

---

## 🎯 Objective
- Predict customer purchase behavior (`Revenue`)
- Use **Python 3.12**
- Implement **K-Nearest Neighbor (k = 1)**
- Evaluate results using **Sensitivity** and **Specificity**

---

## 🧠 Machine Learning Approach
- **Model:** K-Nearest Neighbor (KNN)
- **Library:** scikit-learn
- **Train/Test Split:** 60% training, 40% testing
- **Target Variable:** Revenue  
  - `1` → Purchase completed  
  - `0` → No purchase  

---

## 📂 Dataset Information
- File: `shopping.csv`
- Total Records: ~12,000 user sessions
- Features include:
  - Page visit counts and durations
  - Bounce rate, exit rate, page value
  - Month, browser, operating system
  - Visitor type and weekend indicator
- Target label: **Revenue**

All categorical values are converted into numeric form for model compatibility.


## ⚙️ Requirements
- Python **3.12**
- scikit-learn

Install required library:
bash
pip install scikit-learn
## ▶️ How to Run
1. Make sure Python 3.12 is installed.
2. Install required dependencies:
bash
pip install scikit-learn
python shopping.py shopping.csv





## 📊 Sample Output
The model produced the following results on the test dataset:

- **Correct Predictions:** 4076  
- **Incorrect Predictions:** 856  
- **True Positive Rate (Sensitivity):** 40.49%  
- **True Negative Rate (Specificity):** 90.04%







## 📈 Evaluation Metrics
- **Sensitivity (True Positive Rate):**  
  Measures the proportion of actual buyers correctly identified by the model.

- **Specificity (True Negative Rate):**  
  Measures the proportion of non-buyers correctly identified by the model.

These metrics are preferred over simple accuracy for imbalanced datasets.
## 🧩 Implemented Functions
The following functions are implemented in `shopping.py`:

- `load_data()`  
  Reads the CSV file, converts categorical values into numeric form, and returns evidence and labels.

- `train_model()`  
  Trains a K-Nearest Neighbor (KNN) classifier with `k = 1` using the training data.

- `evaluate()`  
  Calculates sensitivity and specificity based on model predictions.
## 👤 Author
**Muhammad Zeeshan Nasrullah**
