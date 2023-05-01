# Credit Risk Classification
![creditrisk](https://github.com/ericyang91/Credit_Risk_Classification/blob/main/creditrisk.jpg)

## Overview of the Analysis

The purpose of the analysis is to use logistic regression to classify good clients from bad clients for lending purposes. The evaluation is based on several factors, including 'loan_size', 'interest_rate', 'borrower_income', 'debt_to_income' ratio, 'num_of_accounts', 'derogatory_marks', and 'total_debt', to decide the 'loan_status' ('0' for good and '1' for bad). The data shows 75,036 good clients and 2,500 bad clients, which serve as the target numbers for our model.

We used two different logistic regression models in our analysis. The first model used raw data to train, fit, and predict, whereas the second model used synthetic balanced data from the RandomOverSampler module to train, fit, and predict. We split the datasets in both models into train and test sets to ensure that we test the models on unseen data.

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

The precision and recall rates above reflect the 'bad' clients ('1') as the focus should be on correctly identifying them. Both models have good rates on all three evaluation criteria. The recommended model, however, is the second model that randomly creates synthetic data in the minority dataset to match the number of the majority dataset. It gives us perfect accuracy and recall scores. The decision on whether to use precision or recall depends on the business goals of the lender. If a rocky road lies ahead, it is crucial to mitigate risk; therefore, the recommended criterion to evaluate the model is recall. On the other hand, if the business is flourishing, we might want to minimize any loss of opportunity. In this case, precision is recommended.

## Languages and Libraries
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-0.24.2-blue)](https://scikit-learn.org/stable/)
[![Python](https://img.shields.io/badge/python-v3.10-blue)](https://www.python.org/downloads/release/python-310/)
[![Pandas](https://img.shields.io/badge/pandas-v1.3.3-blue)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-v1.21.4-blue)](https://numpy.org/)

