## Logistic Regression

Here we write a code from scratch to train logistic regression for the data given in the [link](https://archive.ics.uci.edu/ml/datasets/Cervical+Cancer+Behavior+Risk)
using stochastic gradient descent.

The batch size is set to 1, learning rate to 0.001 and the number of iterations 
to 1000. The dataset is used for a binary classification task. We have splitted the data into 90% and 10% sets, where 10% 
set is the test set. 

Finally we compare the performance of our implementation to that of logistic regression 
available in sklearn.

The `result.txt` file contains the accuracies of the two models.
