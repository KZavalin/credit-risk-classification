# Module 12 Report Template

## Overview of the Analysis
In this challenge, I completed analysis of a lending data database to complete a machine learning model that predicts healthy versus high-risk loans based on  multiple variables that included: loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, and total debt amount. Two separate meachine learning models were created. For the first model, the data was split into X list of the aforementioned variables used for the prediction, and Y outcome of each loan status. These data were split into a training and test databases, which were used to train and then test the data using a logistic regression model. For the second model, the same process was used, but the training dataset was resampled to represent an equal number of healthy and high-risk loans to deal with an unproportionally larger number of healthy vs high risk loans in the original dataset. 

## Results
* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
* Model 1 Balanced Accuracy was .95
* Healthy loans were identified with
  * Precision: 1.00
  * Recall .99
* High-risk loans were identified with
  * Precision .85
  * Recall .91

* Machine Learning Model 2:
* Model 1 Balanced Accuracy was .99
* Healthy loans were identified with
  * Precision: 1.00
  * Recall .99
* High-risk loans were identified with
  * Precision .84
  * Recall .99
## Summary


I
For the first model, prediction of healthy loans was good with 99% recall - that is, majority were correctly identified. However, high-risk loans were predicted not as successfully. The 91 recall indicates that about 10% of high-risk loans in the test dataset were not correctly predicted, and only 85% of predicted high-risk loans were actually high-risk loans. 

For the second model (rebalanced), healthy loans were predicted very well, will 100% precision and 99% recall. However, high-risk loans were not predicted as well. While recall was 99% (most high-risk loans are identified), 84% accuracy showed that a significant percentage (16%) of loans identified as high-risk were actually healthy loans. However, the actual number of mislabeled healthy loans represents only a very small percentage of healthy loans, which were typically properly identified (healthy loans have 99 recall). Therefore, this is a suitable model, as it identifies the vast majority of high-risk loans, which is the critical task for this model, and leaves the majority of healthy loans out of this group. Nonetheless, there will be rare occasions of healthy loans being misidentified as high-risk.

The balanced accuracy also reflects the merits of the second model, which has a high score of 99% accuracy vs the poorer 95% accuracy of the first model. 