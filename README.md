# Credit Card Fraud Detection

## Overview
This project focuses on detecting fraudulent credit card transactions using supervised machine learning techniques.  
The dataset used is highly imbalanced, containing a majority of non-fraudulent transactions.  
To address this, undersampling was applied to balance the dataset before training multiple classification models.

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Workflow

### 1. Data Loading
- Loaded the dataset `creditcard.csv`.
- Inspected dataset structure and missing values using `df.info()` and `df.describe()`.

### 2. Exploratory Data Analysis (EDA)
- Visualized the distribution of `Amount` using **KDE** and **boxplots**.
- Observed severe class imbalance in the `Class` column.

### 3. Data Balancing
- Applied **undersampling** to reduce the number of valid transactions to match the number of fraud cases.
- Created a new balanced dataset.

### 4. Model Training
- Split the data into training and testing sets.
- Trained multiple models:
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
- Evaluated models using confusion matrices and accuracy scores.

### 5. Evaluation
- Metrics used:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-Score  
  - Confusion Matrix  

---

##  Problems Faced &  Solutions

Problem 1 : Imbalanced Dataset

Issue:
The dataset contained very few fraud cases, causing models to be biased toward non-fraud predictions.

Solution:
Applied undersampling to create a balanced dataset of fraud and valid transactions.

Problem 1: Imbalanced Dataset

Issue:
The dataset contained very few fraud cases, causing models to be biased toward non-fraud predictions.

Solution:
Applied undersampling to create a balanced dataset of fraud and valid transactions.

Problem 2:
The dataset provided by the company contained hidden or anonymized features (e.g., V1, V2, ..., V28).
Because of this, it was impossible to understand the real meaning of each feature or determine their business relevance.
This also made feature selection and interpretability challenging.

Solution:

Treated all anonymous features as numerical inputs and applied scaling (StandardScaler) to normalize them.

Relied on correlation analysis, model-based feature importance (RandomForest feature_importances_), and statistical tests to select relevant features.

Focused on model performance metrics (precision, recall, F1-score) rather than feature interpretation.
-------------------------------------------------------------------------------------------------------------------------------
👤 Author
Shreyash Ekawade
Machine Learning | Data Analytics 
GitHub Profile
