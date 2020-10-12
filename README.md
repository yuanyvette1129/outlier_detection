# outlier_detection

About the data
The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Project Goal
Identify fraudulent credit card transactions.

Results
Distribution-based modeling reach a F1 score = 0.74

Trained Supervised ML (Random Forest) with SMOTE sampling technique improved F1 score from 0.82 to 0.85.

Added the predicted probability feature from the distribution-based modeling, and got an F1 score of 0.83 using Random Forest (with SMOTE, improved to 0.84)

I also tried unsupervised algorithm isolation forest, which gives a F1 score = 0.36
