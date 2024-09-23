# credit-risk-classification
Supervised Learning practice

RISK ANALYSIS REPORT
The purpose of this analysis is the evaluate loans and how likely they are to default.  We were given bank data that held many variables, but most importantly had status default status on each loan, this was key to train the data using a supervised approach. We used the information: loan size, interest rate, borrower's income, debt to income ratio, number of accounts, total debt, and previous derogatory marks to determine the likelyhood a loan would default.

In the machine learning process we first split the data into labels and features.  The Loan Status was our label, or target.  The rest were features.  We then split the data into training and testing groups using train_test_split.  We then fit the model and made predictions us ign more SKlearn features.  Finally we made a confusion matrix and ultimately a classification report.

Machine Learning Model 1: Logistic Regression
--Accuracy: 99%
--Precision (for class 1): 0.85
--Recall (for class 1): 0.95
--F1-Score (for class 1): 0.89
--The logistic regression model performed well with high accuracy and strong recall for the minority class (class 1), although precision for class 1 could be improved.

The Logistic Regression model performed the best overall in terms of balancing precision, recall, and F1-score for both classes. It is particularly important in this problem to predict class 1 (defaulted loans) accurately, as failing to do so could lead to significant financial loss. The model had strong recall for this class, meaning it successfully identified most of the defaulted loans. Based on the results, I recommend using the Logistic Regression model, as it provides the best trade-off between accuracy and recall for this problem. If further fine-tuning is required, efforts should be made to improve the precision for class 1.