# Titanic_ML_Project

Overview

This project focuses on predicting whether a passenger on the Titanic would have survived using basic machine learning techniques. I worked with the classic Titanic dataset and implemented a logistic regression model to classify survival outcomes based on selected passenger features.

Dataset Description
The dataset contains passenger-level information such as:
- Age
- Gender
- Travel class (Pclass)
- Fare
- Family members aboard (SibSp, Parch)
- Embarkation port
  
The target variable is Survived, which is binary (0 = did not survive, 1 = survived).

Preprocessing
Key preprocessing steps included:
- Dropping irrelevant features like PassengerId, Name, Ticket, and Cabin
- Handling missing values, particularly in Age
- Encoding categorical variables:
- Sex mapped to 0 and 1
- Embarked converted to one-hot encoded columns
- Verifying all features were numeric before training
  
Model Used
I trained a logistic regression model using scikit-learn. The dataset was split into 80% training and 20% testing using train_test_split.

Setup & Installation

Make sure you have the following installed:
pip install pandas numpy matplotlib seaborn scikit-learn

Running the Code

Download the Titanic dataset from Kaggle
Place the CSV files (train.csv, test.csv) in your working directory
Run the preprocessing, training, and prediction steps in your notebook or script

Results
- Model trained successfully without string-type errors
- Training and test accuracy were computed using accuracy_score
- Predicted values matched well with expected outputs
