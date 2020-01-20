# Logistic-Regression
The classification goal is to predict whether the client will subscribe (1/0) to a term deposit (variable y).
The dataset comes from the UCI Machine Learning repository, and it is related to direct marketing campaigns (phone calls) of a Portuguese banking institution.

Logistic Regression is a Machine Learning classification algorithm that is used to predict the probability of a categorical dependent variable. In logistic regression, the dependent variable is a binary variable that contains data coded as 1 (yes, success, etc.) or 0 (no, failure, etc.). In other words, the logistic regression model predicts P(Y=1) as a function of X.

# Logistic Regression Assumptions
1) Binary logistic regression requires the dependent variable to be binary.

2) For a binary regression, the factor level 1 of the dependent variable should represent the desired outcome.

3) Only the meaningful variables should be included.

4) The independent variables should be independent of each other. That is, the model should have little or no multicollinearity.

5) The independent variables are linearly related to the log odds.

6) Logistic regression requires quite large sample sizes.

# SMOTE algorithm
SMOTE algorithm(Synthetic Minority Oversampling Technique) is used for the over sampling purpose.It creates synthetic (not duplicate) samples of the minority class. Hence making the minority class equal to the majority class. SMOTE does this by selecting similar records and altering that record one column at a time by a random amount within the difference to the neighbouring records.At a high level, SMOTE:

1) Works by creating synthetic samples from the minor class (no-subscription) instead of creating copies.

2) Randomly choosing one of the k-nearest-neighbors and using it to create a similar, but randomly tweaked, new observations.

# Recursive Feature Elimination
Recursive Feature Elimination (RFE) is based on the idea to repeatedly construct a model and choose either the best or worst performing feature, setting the feature aside and then repeating the process with the rest of the features. This process is applied until all features in the dataset are exhausted. The goal of RFE is to select features by recursively considering smaller and smaller sets of features.

# ROC Curve
ROC curves typically feature true positive rate on the Y axis, and false positive rate on the X axis. This means that the top left corner of the plot is the “ideal” point - a false positive rate of zero, and a true positive rate of one. This is not very realistic, but it does mean that a larger area under the curve (AUC) is usually better.
