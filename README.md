# Credit Risk Classification

## Overview of the Analysis

The purpose of the analysis is to use logistic regression in order to classify the good clients from the bad clients for lending purposes. The evaluation was based on the 'loan_size', 'interest_rate', 
'borrower_income', 'debt_to_income' ratio, 'num_of_accounts', 'derogatory_marks', and 'total_debt' to decide the 'loan_status' ('0' for good and '1' bad).
The data showed 75,036 good clients and 2,500 bad clients, which served as the target numbers for our model.

We used two different logistic regression models in our analysis. The first model used the raw data to train, fit, and predict whereas the second model used a synthetic balanced data from RandomOverSampler module to 
train, fit, and predict.
The data sets in both models were split into train and test sets in order to make sure we test the models on unseen data.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    - `Accuracy: 0.88`
    - `Precision: 0.87`
    - `Recall: 0.89`


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
      - `Accuracy: 1.00`
      - `Precision: 0.87`
      - `Recall: 1.00`

## Summary

The above precision and recall rates reflect the 'bad' clients ('1') as the focus should be to correcly identify them. Both models have good rates on all three evaluation criterias. The recommended model, however, is the second model that randomly creates synthetic data in the minority data set to match the number of the majority data set. It gives us perfect accuracy and recall scores.
Decision whether to use precision or recall depends on the business goals of the lender. If a rocky road lies ahead, it is crucial to mitigate risk, therefore the recommended criteria to evaluate the model is recall. On the other hand, if the business is flourishing, we might want to minimize any loss of opportunity. In this case, precision is recommended.
