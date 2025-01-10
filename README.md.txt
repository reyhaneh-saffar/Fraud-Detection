# Fraud Detection

## Overview
This project focuses on detecting fraudulent transactions in a simulated credit card transaction dataset. The dataset spans transactions from **1st Jan 2019 to 31st Dec 2020**, containing records from **1,000 customers** and **800 merchants**.

---

### 1. **Data Exploration**
- Comprehensive analysis of the dataset to understand its structure and identify patterns.
- Ensured **no null values** in both numerical and categorical columns, highlighting the dataset's integrity.

### 2. **Data Processing**
#### Null Value Analysis
- Inspected each column for unique values, null counts, and data types.
- Found all columns complete with no missing data, ensuring a solid foundation for analysis.

#### Sampling
- **Balanced dataset creation:**  
  - Used **stratified sampling** to address class imbalance.
  - Fraudulent transactions were paired with a proportionate sample of non-fraudulent transactions.
- Applied **RandomUnderSampler** to further balance the training dataset.

#### Data Scaling
- Standardized numerical features using `StandardScaler`.
- Ensured uniformity in feature scales for improved model performance.

#### Data Encoding
- Applied **One-Hot Encoding** to categorical variables.
- Expanded the feature space to capture categorical information effectively.

---

### 3. **Model Evaluation**
- Tested multiple classification algorithms:
  - **Logistic Regression**
  - **LinearSVC**
  - **K-Nearest Neighbors (KNN)**
  - **Decision Tree**
  - **Random Forest**
  - **Naive Bayes**

#### Evaluation Metrics:
- **Accuracy**: Measures overall prediction correctness.
- **AUC (Area Under ROC Curve)**: Assesses discriminatory power.
- **F1 Score**: Balances precision and recall.

#### Results:
- **Best-performing model:** Random Forest  
  - Accuracy: **82.81%**  
  - AUC: **78.97%**  
  - F1 Score: **43.99%**
- ROC curves were plotted to visualize model performance, saved as `roc_curve.eps`.

---
