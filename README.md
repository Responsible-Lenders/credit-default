# credit-default
A project on predicting default of credit card clients.


Logistic Regression:

  Logistic regression is a linear model for classification, in which a sigmoid function is used to predict the probability of a discrete outcome for a given set of features. The sigmoid is fitted to the training set which then predicts the outcome in the test set based on a chosen cutoff value. Classification metrics such as precision and recall vary differently as a function of the cutoff, allowing the model to be tailored to maximize the most relevant metrics.
  Here we implemented the logistic regression function from scikit learn with two different solving algorithms, “L-BFGS” and “liblinear”. The elements of the confusion matrix were found which were used to calculate the accuracy, precision, recall and F1 scores as a function of the cutoff. Overall “liblinear” performed better than “L-BFGS”, with an F1 Score of 50% and an Accuracy of 81% when the cutoff ranges from 0.25 and 0.4. Given the class imbalance of 78% non-default to 22% default, this constitutes a 3% increase in Accuracy and 50% increase in F1 Score compared predicting non-default in every case. Other metrics were calculated such as Negative Predictive Value and Specificity.
