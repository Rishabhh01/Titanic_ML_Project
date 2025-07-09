# Titanic_ML_Project

## Overview

This project predicts the survival of Titanic passengers using a baseline **logistic regression** classifier built with `scikit-learn`. It walks through data cleaning, feature engineering, model training, and evaluation, serving as a clear introduction to supervised classification on a real-world dataset.

**Dataset (Kaggle):**  
https://www.kaggle.com/c/titanic

## Dataset Description

Each record represents one passenger and contains:

- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Sex`: Gender (male/female)
- `Age`: Age in years
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Fare`: Passenger fare
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

**Target Variable:**  
- `Survived`: 0 = Did not survive, 1 = Survived

## Preprocessing Pipeline

1. **Drop Non-Predictive Columns**  
   - `PassengerId`, `Name`, `Ticket`, `Cabin`

2. **Handle Missing Values**  
   - `Age`: Filled with median value  
   - `Embarked`: Filled with the most frequent category

3. **Encode Categorical Variables**  
   - `Sex`: Mapped to 0 (male) and 1 (female)  
   - `Embarked`: One-hot encoded into `Embarked_C`, `Embarked_Q`, and `Embarked_S`

4. **Verify All Features Are Numeric**  
   - Ensured the feature matrix is fully numeric before feeding into the model

## Model

- **Algorithm**: Logistic Regression  
- **Library**: `scikit-learn`  
- **Data Split**: 80% training / 20% testing using `train_test_split`  
- **Evaluation Metric**: Accuracy

## Setup and Installation

Ensure Python and pip are installed on your machine, then install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```   

## Results

- Model trained successfully without string‑type errors  
- All categorical features were encoded correctly  
- Predictions aligned well with the actual outcomes  

**Example Accuracy Scores**

- Training Accuracy: ~0.80  
- Test Accuracy: ~0.79  

---
## Author
**Rishabh Chauhan**  
Email: rishabhc2234@gmail.com


