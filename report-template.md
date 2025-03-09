# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

Lending organizations give loans to borrowers in the hope that the borrower would either pay back the lender or return the asset. Credit risk is the possibility that a borrower may fail to repay a loan or return an asset, which would result in a loss for the lender. However, in order to develop a model that can determine borrowers' creditworthiness, I will employ machine learning to examine a dataset of past loan activity from a peer-to-peer lending services company.

- Based on the loan status that the lending firm provides, I will attempt to use a machine learning model to identify which loans are healthy (low-risk) or non-healthy (high-risk).
    - Since the Logistic Regression Algorithm is frequently used to predict the likelihood of a target variable in classification issues, it is the ideal tool to employ for our machine learning model.

- Using the loan company's the data set, I developed a Logistic Regression Model that produced a 99% accuracy rating. The recall value (0.91) for non-healthy loans is lower than the recall value (0.99) for healthy loans, despite the model's high accuracy. This suggests that the model will be more accurate in predicting loan statuses as healthy than as non-healthy. The imbalance in the dataset, which means that the majority of the data falls into one class label (in this example, healthy loans significantly exceeded non-healthy loans), is the cause of this.

'# code
y.value_counts()

'# output
loan_status
0    75036
1     2500
Name: count, dtype: int64


In accordance with step 3's confusion matrix [Create an LRM with Original Imbalanced Data]:

- The model accurately identified 18,663 of the 18,765 healthy (low-risk) loan statuses and wrongly identified 102.
- The model successfully forecasted 563 of the 619 non-healthy (high-risk) loan statuses as non-healthy, whereas it mispredicted 56 of them.


## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
