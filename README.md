# Breast Cancer Prediction using Machine Learning

## Project Overview
This project uses the Breast Cancer Wisconsin dataset from scikit-learn to predict whether a tumor is malignant (cancerous) or benign (non-cancerous).

## Dataset
- Source: scikit-learn Breast Cancer Dataset
- Samples: 569
- Features: 30 numerical features
- Target:
  - 0 = Malignant
  - 1 = Benign

## Models Used
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Pipeline
- GridSearchCV

## Workflow
1. Data Loading
2. DataFrame Creation
3. Train-Test Split
4. Model Training
5. Model Evaluation
6. Cross Validation
7. Pipeline Implementation
8. Hyperparameter Tuning using GridSearchCV
9. Feature Importance Analysis
10. Model Saving using Pickle

## Results

### Base Models

| Model | Accuracy |
|---------|---------|
| Logistic Regression | 0.9649 |
| Decision Tree | 0.9167 |
| Random Forest | 0.9693 |

### Pipeline Results

| Pipeline Model | Accuracy |
|---------------|----------|
| Logistic Regression Pipeline | 0.9825 |
| Random Forest Pipeline | 0.9708 |

### GridSearchCV Result

| Best Model | Accuracy |
|------------|----------|
| Tuned Random Forest | 0.9766 |

## Feature Importance

Top Important Features:
- Worst Concave Points
- Mean Concave Points
- Worst Area
- Worst Perimeter
- Worst Radius

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Jupyter Notebook

## Files
- `cancer.ipynb` – Complete notebook
- `cancer_model.pkl` – Saved trained model

## Key Learnings
- Classification Problems
- Train-Test Split
- Cross Validation
- Pipeline
- Random Forest
- Feature Importance
- Hyperparameter Tuning with GridSearchCV
- Model Serialization using Pickle

## Future Improvements
- ROC-AUC Score
- Streamlit Deployment
- Flask/FastAPI Deployment
- Model Comparison on Additional Datasets
