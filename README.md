# Titanic Survival Prediction

## Problem
Binary classification — predict whether a passenger survived the Titanic disaster.

## Dataset
- 891 training samples, 11 features
- Source: Kaggle Titanic Competition

## Approach
1. Exploratory Data Analysis
2. Preprocessing — missing value imputation, encoding, scaling
3. Trained 3 models: Logistic Regression, Random Forest, SVC
4. Evaluated using F1 score (chosen over accuracy due to class imbalance)
5. Tuned best model with GridSearchCV

## Results
| Model | F1 Score |
|---|---|
| Logistic Regression | 0.7244 |
| Random Forest | 0.7287 |
| SVC | 0.7167 |
| Random Forest (Tuned) | 0.7188 |

## Key Decisions
- Dropped Cabin (77% missing)
- Used F1 over accuracy — classes are imbalanced (62/38)
- Used median imputation for Age to avoid outlier influence

## Tech Stack
Python, Scikit-learn, Pandas, NumPy
