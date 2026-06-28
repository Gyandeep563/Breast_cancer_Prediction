# Breast Cancer Prediction using Machine Learning

## Project Overview

This project predicts whether a breast tumor is **Malignant (Cancerous)** or **Benign (Non-Cancerous)** using Machine Learning techniques. The Breast Cancer Wisconsin dataset from Scikit-Learn was used to train, evaluate, and compare multiple classification models.

The project covers the complete machine learning workflow from data preprocessing to model evaluation and hyperparameter tuning.

---

## Dataset Information

- **Dataset:** Breast Cancer Wisconsin Dataset
- **Source:** Scikit-Learn
- **Samples:** 569
- **Features:** 30 Numerical Features
- **Target Classes:**
  - **0 → Malignant**
  - **1 → Benign**

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook
- Pickle

---

## Project Workflow

1. Data Loading
2. DataFrame Creation
3. Exploratory Data Analysis (EDA)
4. Train-Test Split
5. Feature Scaling
6. Model Training
7. Model Evaluation
8. Cross Validation
9. Pipeline Implementation
10. Hyperparameter Tuning using GridSearchCV
11. Feature Importance Analysis
12. Model Serialization using Pickle

---

## Models Implemented

### Logistic Regression

| Model | Accuracy |
|---------|----------|
| Logistic Regression | **96.49%** |

---

### Decision Tree

| Model | Accuracy |
|---------|----------|
| Decision Tree Classifier | **91.67%** |

---

### Random Forest

| Model | Accuracy |
|---------|----------|
| Random Forest Classifier | **96.93%** |

#### Feature Importance

Top important features identified by Random Forest:

- Worst Concave Points
- Mean Concave Points
- Worst Area
- Worst Perimeter
- Worst Radius

---

### Pipeline Results

| Pipeline Model | Accuracy |
|----------------|----------|
| Logistic Regression Pipeline | **98.25%** |
| Random Forest Pipeline | **97.08%** |

---

### GridSearchCV Results

| Tuned Model | Accuracy |
|-------------|----------|
| Tuned Random Forest | **97.66%** |

---

### Support Vector Machine (SVM)

#### Accuracy Comparison

| Model | Accuracy |
|---------|----------|
| SVM (Without Scaling) | **94.74%** |
| SVM (With Scaling) | **98.25%** |

#### Kernel Comparison

| Kernel | Accuracy |
|---------|----------|
| Linear | **97.37%** |
| RBF | **98.25%** |
| Polynomial | **86.84%** |

#### GridSearchCV Best Parameters

```python
{
    'C': 1,
    'gamma': 'scale',
    'kernel': 'rbf'
}
```

#### Cross Validation Score

```text
97.58%
```

---

## Model Evaluation Techniques

### Confusion Matrix

Used to evaluate:

- True Positives (TP)
- True Negatives (TN)
- False Positives (FP)
- False Negatives (FN)

### Classification Report

Metrics Used:

- Precision
- Recall
- F1-Score
- Accuracy

### Cross Validation

Used 5-Fold Cross Validation to obtain more reliable performance estimates.

### GridSearchCV

Used for automatic hyperparameter tuning and model optimization.

---

## Files Included

```text
cancer.ipynb              -> Main project notebook
SVm_breast_cancer.ipynb   -> SVM implementation notebook
cancer_model.pkl          -> Saved trained model
README.md                 -> Project documentation
```

---

## Key Learnings

Through this project, I learned:

- Classification Problems
- Exploratory Data Analysis (EDA)
- Train-Test Split
- Feature Scaling
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Pipeline
- Cross Validation
- GridSearchCV
- Hyperparameter Tuning
- Feature Importance
- Model Serialization using Pickle

---

## Results Summary

| Model | Accuracy |
|---------|----------|
| Logistic Regression | 96.49% |
| Decision Tree | 91.67% |
| Random Forest | 96.93% |
| Logistic Regression Pipeline | 98.25% |
| Random Forest Pipeline | 97.08% |
| Tuned Random Forest | 97.66% |
| SVM (RBF Kernel) | **98.25%** |

---

## Best Performing Models

🏆 **Logistic Regression Pipeline** — 98.25%

🏆 **SVM (RBF Kernel)** — 98.25%

Cross Validation Score (SVM): **97.58%**

---

## Future Improvements

- ROC-AUC Score Analysis
- Streamlit Deployment
- Flask/FastAPI Deployment
- XGBoost Implementation
- Feature Selection Techniques
- Model Comparison on Additional Datasets

---

## Author

**Gyandeep**

GitHub: https://github.com/Gyandeep563

---

⭐ If you found this project useful, consider giving it a star.
