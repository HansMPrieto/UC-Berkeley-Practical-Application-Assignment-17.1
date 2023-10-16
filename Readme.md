In this project, our goal was to compare the performance of several different classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines (SVC)). The dataset that we used here was related to the marketing of bank products over the telephone. The data came from a Portugese banking institution that developed a marketing campaign for clients to subscribe a term deposit in their bank offering good interest rates. 17 marketing campaigns were conducted between May 2008 and November 2010, corresponding to a total of 79354 contacts. There were 6499 successful subscriptions, which was equivalent to an 8% success rate.

A subset of the contacts consisted of seven categories, which were age, job type, marital status, education level, history of credit default, housing loan status, and personal loan status. The target variable wa whether or not the contact was successful in subscribing a term deposit. 88.73% of the contacts for this subset had no success. 11.27% of the contacts were successful.

Age was the only numerical predictor variable. There were no separate populations for the success categories. Thus, age does not have a strong predictive value on the success of the contact.

The six categorical predictor values were job type, marital status, education level, history of credit default, housing loan status, and personal loan status. The job type variable had a chi-square value of 22.383324, and the education level variable had a chi-square value of 23.732190. Marital status had a chi-square value of 8.012887, history of credit default had a chi-square value of 3.225474, housing loan status had a chi-square value of 2.463106, and personal loan status had a chi-square value of 0.194872. Since job type and education level had the highest chi-square values, it can be implied that job and education have the most influence on the success of a contact subscribing a term deposit.

The baseline model consits of classifying all data as 'no' success. If all data were classified as 'no', the model would have an accuracy rate of 88.73%. he model doesn't classify any observations as positive, so precision and recall are zero percent.

The logistic regression model did not classify any observations as 'yes' for success. The KNN, Decision Tree, and SVC models were slightly less accurate than the baseline model. However, they showed improvements in the precision and recall metrics.

The Decision Tree model correctly predicted the most 'yes' contacts. Thus, recall is the most useful metric.


Factors that were most important in the success of a contact:
- A client having no history of a credit default is more likely to accept a subscription
- Married and divorced clients were less likely to accept a subscription.

In terms of next steps and recommendations, recall is likely a more useful metric. Models can be improved using recall as the metric to select an optimum model.