# Credit-Risk-Estimation-and-Strategy (Neural Network and XGBoost)
High performance machine learning model using Python to predict if the customer will default in credit payments and calculate the risk associated. Devised an aggressive and a conservative strategy to approve credits to customers based on their probability of defaulting. Used grid-search for Neural Network and XGBoost algorithms for model training and optimization.

Data used- American Express (Kaggle Competition - Default Prediction) : https://www.kaggle.com/competitions/amex-default-prediction/data

Steps followed -
1. Filtering from the 7M records and joining with default labels.
2. Data Exploration
3. One Hot Encoding
4. Feature Selection (Feature importance calculated by running an XGB Model)
5. Train and Test split sample
6. XGB Model fit to verify feature importance and filter features
7. Grid Search for XGBoost model
    - 	Number of trees: 50, 100, and 300
    - 	Learning Rate: 0.01, 0.1
    - 	Percentage of observations used in each tree: 50%, 80%
    - 	Percentage of features used in each tree: 50%, 100%
    - 	Weight of default observations: 1, 5, 10
8. Best XGB model selection
9. Pre-processing for Neural Networks (Missing value imputation, outlier treatment 1-99 percentile, standardization)
10. Grid Search for Neural Network model
    - 	Number of hidden layers: 2, 4
    - 	Nodes in each hidden layer: 4, 6
    - 	Activation funciton for each hidden layers: ReLu, TanH
    - 	Dropout regularization for hidden layers: 50%, 100% (no dropout)
    - 	Batch size: 100, 10000
11. Best NN model selection
  
