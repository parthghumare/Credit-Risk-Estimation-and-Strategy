# Credit-Risk-Estimation-and-Strategy
High performance machine learning model using Python to predict if the customer will default in credit payments and calculate the risk associated. Devised an aggressive and a conservative strategy to approve credits to customers based on their probability of defaulting. Used grid-search for Neural Network and XGBoost algorithms for model training and optimization.

Data used- American Express (Kaggle Competition - Default Prediction) : https://www.kaggle.com/competitions/amex-default-prediction/data

Steps followed -
1. Filtering from the 7M records and joining with default labels.
2. Data Exploration
3. Missing value Imputation, One Hot Encoding 
4. Feature Selection (Feature importance calculated by running an XGB Model)
5. XGB Model fit to verify feature importance and filter features
6. Grid Search for XGBoost model
    - 	Number of trees: 50, 100, and 300
    - 	Learning Rate: 0.01, 0.1
    - 	Percentage of observations used in each tree: 50%, 80%
    - 	Percentage of features used in each tree: 50%, 100%
    - 	Weight of default observations: 1, 5, 10
7. Best model selection
  
  
