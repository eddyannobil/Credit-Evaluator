# supervised-machine-learning


In this assignment, a machine learning model was built that attempts to predict whether a loan from LendingClub will become high risk or not.

Background
LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. 
LendingClub offers their previous data through an API.
This data was used to create machine learning models to classify the risk level of given loans. 
Specifically, a comparison between the Logistic Regression model and Random Forest Classifier.

The Resources folder contains two CSVs that was downloaded from LendingClub:

2019loans.csv
2020Q1loans.csv

An entire year's worth of data (2019) is used to predict the credit risk of loans from the first quarter of the next year (2020).

Preprocessing: Convert categorical data to numeric
A training set was created from the 2019 loans using pd.get_dummies() to convert the categorical data to numeric columns. Similarly, a testing set was also created from the 2020 loans, also using pd.get_dummies(). 

Two models were created and compared on this data: a logistic regression, and a random forests classifier. 

StandardScaler was used to scale the training and testing sets before re-fitting the LogisticRegression and RandomForestClassifier models on the scaled data to make another prediction and assess how scaling affects the accuracy of the models. 