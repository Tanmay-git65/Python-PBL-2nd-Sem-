# Heart Disease Prediction using Machine Learning

## Overview

This project is developed as part of a Project-Based Learning (PBL) initiative.
The goal is to predict the presence of heart disease using machine learning techniques based on patient health data.

The project is divided into multiple phases including data cleaning, exploratory analysis, and model building.

---

## Project Structure

```
AIML-PBL/
│── Phase 1/
│     └── data_cleaning.ipynb
│── Phase 2/
│     └── EDA.ipynb
│── Phase 3/
│     └── main.ipynb
│── dataset/
│     └── heart_disease_prediction_raw.csv
```

---

## Phase-wise Breakdown

### Phase 1: Data Cleaning

* Loaded raw dataset
* Removed duplicate records
* Handled missing values:

  * Dropped missing target values
  * Filled categorical with mode
  * Filled numerical with median
* Dropped unnecessary columns (e.g., `id`)
* Standardized categorical values
* Converted data types
* Removed outliers using IQR method
* Exported cleaned dataset

---

### Phase 2: Exploratory Data Analysis (EDA)

* Analyzed feature distributions
* Used boxplots for outlier detection
* Used bar charts and cross-tabulation for categorical analysis
* Identified relationships between features and target variable

---

### Phase 3: Model Building & Evaluation

#### Data Preprocessing

* Encoding:

  * Label encoding for binary categories
  * One-hot encoding for multi-class features
* Feature scaling using StandardScaler
* Train-test split (80-20)

---

## Machine Learning Models Used

### 1. Logistic Regression

* Used for binary classification
* Implemented feature selection using coefficient importance
* Iteratively removed least important features
* Final model trained on optimized feature set

---

### 2. K-Nearest Neighbors (KNN)

* Used k = 5
* Distance-based classification
* Evaluated using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
  * ROC-AUC

---

### 3. Support Vector Machine (SVM)

* Kernel used: RBF
* Enabled probability predictions
* Evaluated using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
  * ROC-AUC

---

## Model Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix
* Classification Report

---

## Results

* Compared Logistic Regression, KNN, and SVM
* Best model selected based on performance metrics
* Visualization of confusion matrices and ROC curves included

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

## How to Run

1. Install dependencies:

```
pip install numpy pandas matplotlib seaborn scikit-learn
```

2. Run Jupyter Notebook:

```
jupyter notebook
```

3. Execute notebooks phase-wise:

* Phase 1 → Data Cleaning
* Phase 2 → EDA
* Phase 3 → Model Training

---

## Key Features of Project

* Complete ML pipeline (raw data → prediction)
* Real-world healthcare dataset
* Feature engineering + selection
* Multiple model comparison
* Visualization-driven insights

---

## Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Deployment using Flask/Streamlit
* Adding more datasets for better generalization
* Deep learning models for comparison

---

## Contributors

* Sparsh Saxena
* Samarth Tomer
* Tanmay Kumar
