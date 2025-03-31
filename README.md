# credit-risk-classification

## Overview of the Analysis

* This project uses a dataset of historical lending activity `lending_data.csv` from a peer-to-peer lending services company to build a model `logistic regression model` that can identify the creditworthiness of borrowers.
* The financial information the data was on are as follows.
    1. Loan Size - Amount of loan
    2. Interest Rate - Percentage of the amount of the loan charged
    3. Borrower Income - Income of the Borrower
    4. Dept to Income - Amount of the dept payed with respect to the income 
    5. Number of Account - Number of the borrower's account
    6. Derogatory Marks - Marks representing bad activities
    7. Total Debt - total dept accross different account of a borrower
    8. Loan Status - status representing healthy loan `0` and high risk loan `1`

    - Among the information the data was on we used loan status as labels which is to be predicted and remaining as features used for the prediction.

* The machine learning process I went through as part of this analysis.
    1. Importing the file and reviewing the information the file was on.
    2. Setting one of the features within the data as labels (loan_status) that is to be predicted and remaining features as predictors
    3. Splitting the data into testing and training datasets.
    4. Creating a Logistic Regression Model
    5. Predicting on the testing data labels by using the testing feature data and the fitted model.
    6. Evaluating the models performance by generating confusion matrix and classification report.

* The method I used is`LogisticRegression` which is used to predict binary outcome based on the features of a dataset. Special function used is sigmoid function.

## Results

- According to the classification report generated in the code, the precision and recall for `0` (healthy loan) are both 1. This means that out of all the predicted healthy loans, they were actually healthy loans, and there were no instances where the model predicted healthy loans as unhealthy loans.

- Regarding `1` (high-risk loan), the precision is 0.87, which means 87% of the predicted high-risk loans were correct, whereas the recall is 0.95, meaning 5% of the high-risk loans were not detected.

## Summary

### Result Evaluation 

- For `0` healthy loan the precision, recall and f1-score for the model we used is 1 which means the model perfectly predicts it.
- For `1` high risk loan the precision is 0.87 which is good and recall is 0.95 which is high which means the model is detecting most of the high risk loans and the amount of high risk loans predicted is actually at high risk is good enough.

### Recommendation 

- Taking a look in the result evaluation, the model seems to predict effectively. Although there is always room for improvement, I would recommend this model.
