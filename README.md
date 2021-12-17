# Customer-Churn-Prediction
This application predicts whether a customer will churn based on some data.
 - Started with exploring data, the project repository has a notebook named 'EDA & Data preprocessing'
 - There are considerable amount of missing values that we have to deal with. For 1.75% of data, the class label that is "churn" variable is missing
 - Then used various imputation techniques to impute feature variables and KNN classification algorithm to impute missing class variable
 - Perform data visualizations to find interesting insights from data.
 - Perform label encoding of categorical variables and standardization for all numerical variable
 - After all this is done, created a reusable pickle file having X_train, X_test,y_train and y_test
 - Also pickle standardization scalar object that is fitted on X_train to perform transformation on unseen data
 - For model building and evaluation, loaded these data and run them with different algorithms in the notebook named "Model building and Evaluation".
 - The performance is found to be good with maximum accuracy of 91% with randomforest and gradientbossting classifier
 - Then pickle the randomforest to make it reusable in an app
 - Finally, created an api with flask that takes data as input perform featurization an use our serialised model to make predictions and give output as whether the customer will churn or not
