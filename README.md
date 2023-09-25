# credit-risk-classification


CREDIT RISK ANALYSIS REPORT

Analysis Overview:

The purpose of the analysis is to help predict the creditworthiness of borrowers.   The model was built on a dataset of historical lending activity from a peer-to-peer lending services company.

The financial information provided included the size of the loans, interest rate, income of the borrower, debt-to-income ratio of the borrower, number of accounts, number of derogatory marks, total debt, and the loan status(healthy or high-risk of default).  The analysis will try to predict the level of risk when evaluating future loan applications.

To complete the analysis I used the Logistics Regression model. After initially reading in the dataset, I separated the 'loan_status' as the y-variable.  Next step as to split the data into training and testing datasets to use in the model.
After splitting the data I fit the model using training data, then completed the predictions step.
To evaluate the model, I first checked the accuracy score, generated a confusion_matrix, and then printed the classification report.


Results:

- Accuracy score:  Accuracy rating of the model is 99%, 

- Precision score:  Healthy loan predictions is at 100%, risky loans at 85%

- Recall score:  Healthy loan recall was 99%, risky loans at 91%

- F1 score:  Healthy loan rating of 100%, but for the high-risk loans it was 88%


Summary:

The logistics regression model predicted a 99% balanced accuracy score, which is great.  The precision and f1-scores for healthy loans was at 100% as well.

For the high-risk loans (loan_status=1) the predictions were less accurate.   Since the data was imbalanced, it is better to use the F1 score to assess the model performance.

The F1 score for high-risk loans is 0.88, which is reduced confidence in accurately predicting that a loan may be high risk.  Using the accuracy score the lender may eliminate or deny more loans than they should.  Relying on the F1 score at 88% may encourage the lender to more closely evaluate those applicants that are near the cutoff to see if other details or references would provide a better picture of loan risk.

