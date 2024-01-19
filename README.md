# credit-risk-classification

In this Challenge, various techniques were used to train and evaluate a model based on loan risk. Data was retried from lending_data.csv. One model was created and evaluated using the original data. Then the data was resampled and an additional Logistic Regression model was created and evaluated. 

## Credit Analysis Report


### Overview of the Analysis

The purpose of this analysis was to predict and identify the creditworthiness of borrowers, by creating and evaluating a model based on the provided data on loan risk. The available data (found in lending_data.csv) contains financial information on loan size and its interest rate, the borrower's income, a debt to income ratio, number of accounts, total debt and finally loan status. The target the model was trained to predict was loan status, denoted as 0 for healthy loan and 1 for high-risk loan. The remaining information was used as features in the model. 

The data, once divided into target and features, was split into testing and training data. The purpose was for the training data to be fitted using a logistic regression model. In the first model, the original training data was fitted. In the second model, the training data was re-sampled and fitted. In both models,  predictions were made against the original testing data. The performance of the models was evaluated by calculating the accuracy and generating a confusion matrix and a classification report. 

### Results 

* Machine learning model 1: 
- With an accuracy score of 95%, the model performed very well in making the correct predictions. 
- Looking at the classification report, the model was more precise are predicting a healthy loan (0) than a high-risk loan (1) - precision of 1.00 vs 0.85 respectively. 
- Similarly, the recall score when predicting a healthy loan was more sensitive to positive observations than when predicting a high-risk loan, as seen with a recall score of 0.99 vs 0.91 respectively. 
- This explains why the f1-score is higher for healthy loans than a high-risk loan - scores of 1.00 and 0.88 respectively. 

* Machine learning model 2: 
- Using the oversampled data, the accuracy score shows the model performed even better at 99% accuracy. 
- Looking at the classification report, this model was, once again, more precise are predicting a healthy loan (0) than a high-risk loan (1) - precision of 1.00 vs 0.84 respectively. 
- The model was as sensitive to positive observations when predicting a healthy loan as a high-risk loan, with a recall score of 0.99 for both. 
- This is reflected in the f1-score which is still slightly higher when predicting a healthy loan than a high-risk loan - score of 1.00 and 0.91 respectively. 

### Summary 
In summary, Model 1 performed well, with a high accuracy score. However, it was more precise and sensitive in predicting healthy loans than high-risk ones, as indicated by the precision and recall scores. Model 2, on the other hand, which used oversampled data, performed even better in terms of accuracy. It maintained a high precision for healthy loans and improved in predicting high-risk loans, achieving equal sensitivity (recall score) for both health and high-risk loans. 

Based on this, Model 2 seems to perform better. It not only has a higher accuracy score but also shows balanced sensitivity in predicting the two types of loans. A model that's equally good at predicting both can provide a more comprehensive understanding of creditworthiness. 
