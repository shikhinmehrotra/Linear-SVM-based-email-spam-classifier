# Linear-SVM-based-email-spam-classifier
This project builds a linear support vector machine (SVM) model to classify emails as spam or ham.

# Data set
The dataset, taken from the UCI ML repository, contains about 4600 emails labelled as 'spam' or 'ham'. The dataset can be downloaded here: https://archive.ics.uci.edu/ml/datasets/spambase

# Data preprocessing
The columns of the raw data set are given as numbers. These column names are manually renamed using the list provided at the UCI website (https://archive.ics.uci.edu/ml/machine-learning-databases/spambase/spambase.names)
The data set is further scaled and checked for null values and none are found.

# Model building
SkLearn's SVC() class is used to build a Support Vector Machine model. The initial model gives an accuracy of 92.8%, a precision value of 92.5% and a recall value of 88.5%.

# Hyperparameter tuning
The hyperparameter C, for a Support Vector Classifier, which controls the 'softness' of the classifier, is tuned using GridSearchCV class and 5-fold cross validation. A graph is plotted to visualise the training and test accuracy with varying values of C. An optimal value of C that optimizes the accuracy is found to be 10, which gives an optimal accuracy for the model of 93.1%.

Further, the hyperparameter C is tuned to optimize other metric apart from accuracy such as precision and recall and different values of C are found to optimize different metrics.
