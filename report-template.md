# Module 12 Report Template

## Overview of the Analysis

Lending organizations give loans to borrowers in the hope that the borrower would either pay back the lender or return the asset. Credit risk is the possibility that a borrower may fail to repay a loan or return an asset, which would result in a loss for the lender. However, in order to develop a model that can determine borrowers' creditworthiness, I will employ machine learning to examine a dataset of past loan activity from a peer-to-peer lending services company.

- Based on the loan status that the lending firm provides, I will attempt to use a machine learning model to identify which loans are healthy (low-risk) or non-healthy (high-risk).
    - Since the Logistic Regression Algorithm is frequently used to predict the likelihood of a target variable in classification issues, it is the ideal tool to employ for our machine learning model.

- Using the loan company's the data set, I developed a Logistic Regression Model that produced a 96% accuracy rating. The recall value (0.94) for non-healthy loans is lower than the recall value (0.99) for healthy loans, despite the model's high accuracy. This suggests that the model will be more accurate in predicting loan statuses as healthy than as non-healthy. The imbalance in the dataset, which means that the majority of the data falls into one class label (in this example, healthy loans significantly exceeded non-healthy loans), is the cause of this.

We can observe that the data is extremely unbalanced by looking at the code in step 3 [Split the Data into Training and Testing Sets] using the value_counts method. Healthy loans [0] make up the majority class, whereas non-healthy loans [1] make up the minority:

![image](https://github.com/user-attachments/assets/4a730be4-b57e-44af-8cdc-8c09ed4a7b47)

In accordance with step 3's confusion matrix [Create an LRM with Original Imbalanced Data]:

- The model accurately identified 18,655 of the 18,765 healthy (low-risk) loan statuses and wrongly identified 110.
- The model successfully forecasted 583 of the 619 non-healthy (high-risk) loan statuses as non-healthy, whereas it mispredicted 36 of them.

![image](https://github.com/user-attachments/assets/ba185eee-af8b-4d53-a60c-405af20ed958)


## Results

-Logistic Regression Model fitted with Imbalanced Data:
                                           
The Imbalanced DataSet was used to fit the Logistic Regression model, which predicted healthy loans 100% of the time and non-healthy loans 84% of the time.

These errors are more likely to occur in a model fitted with unbalanced data:
- A low-risk, healthy loan is categorized as a high-risk, non-healthy loan.
- A healthy loan is one that is low risk, while a non-healthy loan is one that is high risk.

The model predicted healthy loans with a 1% error rate and non-healthy loans with a 6% error rate, based on the recall scores.

![image](https://github.com/user-attachments/assets/cc52cefa-8834-4a7c-8bf4-fbe944eac078)

Although the model produced a 96% accuracy score, the dataset's imbalance might be fixed.

![image](https://github.com/user-attachments/assets/68fcfe9c-7aaf-4915-894e-0132c2a45a7f)

## Summary

- A lender may desire a model that mandates that healthy and non-healthy loans be correctly classified the majority of the time:
- A lending organization may incur higher costs if healthy loans are labeled as non-healthy loans because it may result in a loss of clients.
- The loss of cash provided by the lender may also make it more expensive for a lending organization to identify non-healthy loans as healthy loans.

Given the significant risk of a lender losing provided funds when classifying non-healthy loans as healthy, the lending business would probably want fewer False Positives. The confusion matrix displays the data, which shows the proportion of healthy and non-healthy loans that the model correctly and incorrectly anticipated.

Fitting a model using unbalanced data

36 (ERRONEOUS FEELINGS) --> The anticipated value is not healthy, whereas the actual value is.

False Negatives (110) --> The expected outcome is healthy, but the actual result is not.
