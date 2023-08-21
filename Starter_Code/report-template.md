# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis was to see the efficiency of the two logistic regression models to see if there is any credit risk linked to the loans. The main focus of this evaluation revolved around the financial data, size of the loan, income of borrower, interest rates, debt-to-income ratio, number of accounts, derogatory marks, and the total debt. The main purpose was to predict if the status of the loan is 0 as in healthy or 1 as in high risk loan. 

The process of machine learning for the analysis goes by the following:

- Split the data into training and testing datasets 
- Create and fit the logistic regression model with the original data 
- Evaluate the model’s performance using the accuracy, precision, and recall scores. 
- Resample the data using the RandomOverSampler to seek out the imbalance
- Do another create and fit logistic regression model with the resampled data
- Evaluate the results of the resample model with the same steps


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

Accuracy:
	overall the accuracy of the model was 94% of the instance

Precision Score:
	the model was 100% precise with a healthy loan even with the model being 87% in the predict 	model.

Recall:
	the model had 100% recall in predicting the healthy loans and 89% for the high-risk loans


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

Accuracy:
	overall the accuracy of the model was 94% of the instance 

Precision Score:
	the model was 99% precise in predicting both healthy and high-risk loans

Recall:
	the model had 99% recall in predicting both healthy and high-risk loans 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

According to the findings, the second logistic regression model, developed with the resampled data, did a better job than the first logistic regression model, developed with the original data, in its ability to predict the high-risk loans. The second model showed higher precision and recall score for the high-risk loans which is a big factor in mitigating financial losses. I believe it is highly recommend to use the logistic regression model with the resampled data when it comes to credit risk analysis. By using this model, the company can effectively evaluate the loan applications and make a well analyzed choice during the loan approval process. 
