# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to use various techniques to train and evaluate models with imbalanced classes. This can be used for credit risk classification, as it is a porblem that is quite prevalent. This is because healthy loans easily outnumber risky loans. The financial information used to conduct this analysis is based on lending data. The parameters considered include the loan size, the interest rate, the borrower's income, total debt, debt to income ratio and the number of accounts they hold. These parameters are used to decide if the loan status is healthy or there is a high risk of defaulting, signified by a 0 and 1 respectively.

The analysis is conducted by predicting a number of variables. Examples include value_counts, used to check the balance of the labels variable. It is used to find labels set from the loan_status column. train_test_split is then used to split the data into training and testing datasets. Finally, a Logistic Regression Model is created with the Original Data, after which the accuracy score is calculaed, a confusion matrix is generated and a classification report is printed. Logistic Regression models are created using the LogisticRegression function. Next, the above steps are repeated by utilising resampled data. The resampling method used in this instance is over sampling, using the RandomOverSampler function. A Logistic Regression Model is again created, this time with the resampled Data, after which the accuracy score is calculaed, a confusion matrix is generated and a classification report is printed.

## Results

* Machine Learning Model 1: Model 1 utilises the original data to create a Logistic Regression model. The results from this model are as follows:
        - Accuracy: 0.9924164259182832
        - Precision: For class purple, 1.00 and for class yellow, 0.87
        - Recall: For class purple, 1.00 and for class yellow, 0.89

* Machine Learning Model 2: Model 2 utilises resampled data using over sampling to create a Logistic Regression model. The results from this model are as follows:
        - Accuracy: 0.994180571103648
        - Precision: For class purple, 0.99 and for class yellow, 0.99
        - Recall: For class purple, 0.99 and for class yellow, 0.99

## Summary

Overall, after comparing the accuracy, precision and recall results, the resampled data using over sampling seems to trump the original data. This is evident by the higher accuracy, precision and recall.

Performance also plays a key role and depends on the problem we are trying to solve. In the example of credit risk classification, it is important to predict the 1s as these have a higher risk of defaulting. So, it is fundamental to gather data regarding this to ensure these loans are not granted.
