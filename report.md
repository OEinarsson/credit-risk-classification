## Overview of the Analysis

* The puurpose of this assignment was to analize data from a  peer to peer lending service and create a logistic regression  model that would identify healthy and at risk loans

* The dataset had the following information rangin  'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income',
       'num_of_accounts', 'derogatory_marks', 'total_debt', and 'loan_status'.
* The balance of the loans in the data was  75036 healthy loans and 2500 at risk loans
* the overall process was; clean the data, train the model, test the model, then validate and report.
* I utilized the logistic regression classification to set the base model, then I used the resampling method to validate the models scores.

## Model 1
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384
## Model 2
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.84      0.99      0.91       619

    accuracy                           0.99     19384
   macro avg       0.92      0.99      0.95     19384
weighted avg       0.99      0.99      0.99     19384

## Summary
Since both  models identify so many healthy loans as risky loans  I cannot recommend its use in a production enviroment as the sole decision making matrix. This would decrease customer trust, and overall lose the company revenue over time. However we could utilize this model to highlight potential risky loans and make a decision with further research, cutting down the potential workload