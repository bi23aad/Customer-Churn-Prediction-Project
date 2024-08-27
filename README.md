Customer Churn Prediction
This project is focused on predicting customer churn using machine learning algorithms like Stochastic Gradient Boosting (SGB), Support Vector Machine (SVM), and Random Forest. My aim is to identify which algorithm performs best in predicting customer and to optimize their performance through hyperparameter tuning. my project compares the effectiveness of these models on a publicly available telecommunication dataset.
Inputs
Dataset:  WA_Fn-UseC_-Telco-Customer-Churn, this is a Churn dataset from Kaggle, it contains 7043 customer records.
Attributes: this dataset contains 21 attributes, categorized into demographic details, account information, service usage metrics etc.
Preprocessing: Data under preprocessing such as handling missing values, encoding categorical variables, and feature scaling.
Outputs
Predictions: the output consist of customer churn prediction, that is if a customer will churn or not based on the data inout.
Performance Metric: Each models performance was evaluated using accuracy, precision, recall, and F1 score.
Parameters in Defined Function
1.	Train_test_split
•	X: this is the features of dataset(independent variables).
•	Y: this is the target variable.
•	random_state: controls the shuffling that is applied to the dataset.
2.	GridSearchCV
•	Parameters:
•	Estimators: SGB, SVM, Random Forest.
•	Param_grid: list of dictionaries with parameter names
•	Scoring: strategy to evaluate the performance of the cross-validation model.
•	Cv: determines the cross-validation splitting strategy.
3.	Fit()
•	X_train: training data.
•	Y_train: target values for training

Findings: Random Forest demonstrated high baseline performance with an accuracy of 85%. SGB showed significant improvement pots-hyperparameter tuning, with 4.94% increase in accuracy. SVM through tuning achieved a modest improvement. After optimization the most reliable for predicting customer churn especially in terms of recall is Stochastic Gradient Boosting(SGB).
