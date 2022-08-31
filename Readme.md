# DETECT FRAUD

Here is an open source dataset from kaggle.com which provides over 6 million entries of bank transfers that are flagged as either fraudlent or non-fradulent. 

"isFraud" column has two variables so we are working with a binary classification. 

Following the notebook, you will see:

1) Imports of Libraries that will be used in development of the model. 

2) Dropping Columns that are irrelevant to our developing model. 

3) Divide our data into X_train, X_test, y_train, y_test (80% training, 20% testing)

3) Because our 'type' column in our Fraud.CSV is categorical but an important element for the model, we fit OneHotEncode our X_train. 

4) Because of the rarity of fraud, SMOTE is incorporated inorder to synthesize entries of the minority class (fraud). SMOTE will analyze patterns and uniformities in these rows and appropriately replicate more samples to feed the algorithms I tested. 

5) Dummy Model as a point of reference, followed by a few others. 

6) Decide on two models to get deeper into - our winners were RandomForestClassifier and DecisionTreeClassifier. 

7) Grid Search our pipelines for rfc and DecisionTreeClassifier.

8) Tune our model based on the best parameters. 

9) Return scores and select Final Model based on performance. 

10) Decision Tree wins.

11) Develop a tool which takes user inputs, stores them into a dictionary, and appropriately formats the dictionary so it can be used in our Final Model to predict whether the entry was fradulent or not. 

12) A grid that shows how the decision tree is working for fun. I think it looks cool! 

ENJOY! 

DATASET -----> https://www.kaggle.com/datasets/miznaaroob/fraudulent-transactions-data

