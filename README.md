# Credit-Card-Fraud-Detection

The datasets contain transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, ... V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.


#OBJECTIVE:
As the sensitive data is masked with PCA components, let's try to figure out under which component or amount the defaults happens the most.

As it is PCA, visualizations are not easy. Let's reduce the dimensions to 2D using T-SNE and see how visuals look. Visuals with hexagon has been updated. So what is hexagon?

The hexagons show the local density of fraudulent transactions (white points). Red colors mean high density of fraud (typically > 75% of points included in the hexagon) whereas blueish colors are associated with a small fraction of fraud.
