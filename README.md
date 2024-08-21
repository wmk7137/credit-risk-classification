# credit-risk-classification
Example Logistic Regression Model used for predicting whether a loan should be considered a healthy or high-risk load based on a person’s previous credit and financial history. The data was sourced from provided financial data in a csv format and split between x data and y data sets. The split x and y data was then converted into test and train x & y variables. The data was then scaled and fit into a logistic regression to predict the likelihood of a healthy or high-risk loan. The model was then tested by a confusion matrix and placed into a classification report for interpretation of accuracy and precision to determine whether the model is viable for use in real world applications.
According to the logistic regression model that was trained, tested, and ran the accuracy and precision of prediction was high for both healthy loans and high-risk loans.  Healthy loans being nearly all identified (99%) and all predicted (100%) with a larger support number (18862).  High-Risk loans were nearly all identified (98%), however only 84% of high-risk loans were actually predicted, they also had a smaller support sample pool of 722, which may have contributed to the lower rate of predictions, due to the smaller sample size.  Based on the overall metric scores of the model (accuracy - 99%, macro avg - 99%, 92%, & 95%, weighted average - 99%, 99%, & 99%). I would use this as a one tool to determine the viability of a loan along with other factors the would be provided at the time of the start of the loan application process.

Healthy Loan      
•	Precision - 0.99
•	recall - 1.00
•	f1-score - 1.00
•	support -18662
High Risk Loan
•	precision - 0.98
•	recall - 0.84
•	f1-score - 0.91
•	support - 722       

                  precision       recall          f1-score       support
      accuracy                                      0.99           19384
     macro avg       0.99         0.92              0.95           19384
  weighted avg       0.99         0.99              0.99           19384

Prediction             Actual
0                        0         18652
1                        1           609
                         0           113
0                        1            10
Name: count, dtype: int64
