# Task 1: Credit Scoring Model - CodeAlpha

## 📋 Project Overview
This project focuses on building a robust **Credit Scoring Model** to predict the likelihood of an applicant defaulting on a loan. By analyzing historical financial data, the model helps financial institutions make data-driven decisions, reducing risk and improving loan approval processes.

## 🎯 Objectives
* Perform comprehensive **Exploratory Data Analysis (EDA)** to understand the features.
* Preprocess the data by handling missing values and scaling numerical features.
* Compare multiple classification algorithms to find the most accurate model.
* Evaluate performance using metrics beyond simple accuracy (Precision, Recall, F1-Score).

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas & NumPy:** For data manipulation and cleaning.
* **Scikit-Learn:** For model building and evaluation.
* **Matplotlib & Seaborn:** For generating analytical graphs.

## 📊 Models Implemented
The following models were trained and compared:
1.  **Logistic Regression:** Baseline statistical model.
2.  **Decision Tree Classifier:** To capture non-linear relationships.
3.  **Random Forest Classifier:** An ensemble method used to improve accuracy and reduce overfitting.

## 📉 Visualizations Included
* **Correlation Heatmap:** To identify relationships between financial variables.
* **Model Comparison Bar Chart:** A side-by-side view of accuracy across different algorithms.
* **Confusion Matrix:** To visualize True Positives and False Positives.
* **ROC-AUC Curve:** To measure the diagnostic ability of the classifier.

## 🚀 Results
The **Random Forest Classifier** achieved the highest performance with:
* **Accuracy:** > 90%
* **ROC-AUC Score:** High discriminatory power between default and non-default cases.

## 📂 File Description
* `credit_scoring.ipynb`: The main Jupyter Notebook containing the code.
* `cs-training.csv`: The dataset used for training and testing.
* `credit_model.pkl`: The serialized version of the best-performing model.

---
**Author:** Raghav Tawri  
**Internship:** Machine Learning at CodeAlpha
