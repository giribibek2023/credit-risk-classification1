# credit-risk-classification1

Machine learning techniques are used to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Factors considered in the analysis included data on:

the size of the loan
its interest rate
the borrower's income
the debt to income ratio
the number of accounts the borrower held
derogatory marks against the borrower
the total debt
The dataset (77,536 data points) was split into training and testing sets. The training set was used to build an initial logistic regression model (Logistic Regression Model 1) using the LogisticRegression module from scikit-learn. Logistic Regression Model 1 was then applied to the testing dataset. The purpose of the model was to determine whether a loan to the borrower in the testing set would be low- or high-risk and results are summarized below.

This intial model was drawing from a dataset that had 75,036 low-risk loan data points and 2,500 high-risk data points. To resample the training data and ensure that the logistic regression model had an equal number of data points to draw from, the training set data was resampled with the RandomOverSampler module from imbalanced-learn. This generated 56,277 data points for both low-risk (0) and high-risk (1) loans, based on the original dataset.


Logistic Regression Model 

Precision: 93% (an average--in predicting low-risk loans, the model was 100% precise, though the model was only 87% precise in predicting high-risk loans)
Accuracy: 94%
Recall: 95% (an average--the model had 100% recall in predicting low-risk loans, but 89% recall in predicting high-risk loans)
