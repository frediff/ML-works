## CNN vs K-NN
The goal of this project (`model_NN.ipynb`) is to classify a sample into two categories as described in the dataset (given 
in this [link](https://archive.ics.uci.edu/ml/datasets/Cervical+Cancer+Behavior+Risk)). We try to compare 
condensed k-nearest neighbour (CNN in short) and simple k-nearest neighbour (k-NN in short) in their ability to classify the points.

We use 15 examples in the dataset as the test set and the remaining examples as the training set. 
For CNN, while condensing, we use only the closest neighbour (1-NN). After condensation, we set the 
value of k to 5 for performing classification on the test data.

The `output.txt` file contains the accuracies of the two models.

