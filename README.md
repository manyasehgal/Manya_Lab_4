# Manya_Lab_4
Random Forest classification workflow in Python with preprocessing, train-test split, and model evaluation.


# Random Forest Classification Workflow

## Overview
This repository demonstrates how to build and evaluate a **Random Forest Classifier** using scikit-learn. The workflow includes data preprocessing, handling missing values, splitting data into training/testing sets, and evaluating model performance with accuracy and classification metrics.

---

## Steps Implemented

### 1. Data Preprocessing
- Dropped the `OBS` column (identifier, not useful for modeling).
- Handled missing values by filling numerical NaNs with the **mean** of their respective columns.

### 2. Feature and Target Definition
- Target variable: `RESPONSE`
- Features: All remaining columns except the target.

### 3. Train-Test Split
- Split dataset into training (70%) and testing (30%) sets.
- Ensured reproducibility with `random_state=42`.

### 4. Model Training
- Used **RandomForestClassifier** from scikit-learn.
- Trained the model on the training set.

### 5. Model Evaluation
- Predictions made on the test set.
- Evaluated using:
  - **Accuracy Score**
  - **Classification Report** (Precision, Recall, F1-score)

---

## Example Output Shapes
```text
Shape of X_train: (rows, features)
Shape of X_test: (rows, features)
Shape of y_train: (rows,)
Shape of y_test: (rows,)
