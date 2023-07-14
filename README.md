# credit-risk-classification
## Overview of the Analysis

This analysis intends to make use of several machine learning techniques to train and assess how well Logistic Regression Models perform at determining a borrower's credit history. The models' results were analyzed after they had been trained using various techniques to determine which model performed better. The numbers 0 (healthy loan) and 1 (high-risk loan) are the model's predictors.

The dataset was split into features and labels, then into training and testing sets, in order to build the models.


- By creating a logistic regression model, training it with the initial training sets (x_train, y_train), fitting it to the training sets, and utilizing it to make predictions, Machine Learning Model 1 was created.
- By resampling the initial training data with the RandomOverSampler module, a logistic regression model was instantiated, fitted to the resampled training sets (x_resample, y_resample), and predictions were made.

Based on the balance accuracy score, confusion matrix, precision, recall, and f1-score in the classification report, each model's performance was calculated.

## Results

- Machine Learning Model 1:
  - Model 1, which was trained on the original data, predicts the two labels with an accuracy of 94.4%. With precision and recall ratings of 1.00, the model does an excellent job of forecasting the healthy loans. The model's capability to identify high-risk loans might be enhanced. Only 87% of real high-risk loans were accurately predicted, according to the precision score for high-risk loans, which is 0.87. The model only correctly recognized 89% of the high-risk loans in the sample, according to the recall score for high-risk loans, which is 0.89.



- Machine Learning Model 2:
  - Model 2 has a 99.6% accuracy rate in predicting the two labels after being trained on the resampled data. With precision and recall scores of 1.00, the model does well at predicting the sound loans. The recall score has increased to 1.00, indicating that the model can now predict all high-risk loans in the dataset, even while the accuracy score for high-risk loans remains at 0.87.


## Summary

According to the analysis, Model 2 looks to be more accurate overall and performs better than Model 1 in predicting high-risk loans. In particular, Model 2 successfully identified every high-risk loan in the dataset while achieving a pretty high precision in high-risk loan prediction, which is regarded as a relatively strong performance in this situation. In order to identify high-risk loans and to generally forecast labels more accurately, I would advise utilizing Model 2.



