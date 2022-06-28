## Neural Networks
### This project consists of two parts:
- **The first part consists of understanding the role of network configuration when 
the number of parameters are kept the same for different configurations.** </br></br>
We designed three different fully connected neural net where each of them have the same 
number of parameters (call it N) and the same number of layers (call it L). L includes all hidden 
layers and the output layer. </br></br>
In the first net (call it ***UniformNet***) each consecutive connecting layers (except the input and the 
first hidden layer) has the same number of parameters. we do some adjustments (if needed) in the last hidden layer only. </br></br>
In the second net (call it ***PyramidNet***), the first two connecting hidden layers have the largest 
number of parameters and then it will decrease gradually with the layer depth. The rate of 
decrease is taken as ½. That is if the first two connecting hidden layers has m parameters, then the next will 
have m/2 parameters and so on. </br></br>
In the third net (call it ***InvPyramidNet***), the first two connecting hidden layers have the smallest 
number of parameters and then it will increase gradually with the layer depth. The rate of 
increase is taken as 2. That is, if the first two connecting hidden layers has m parameters, then the next 
will have 2m parameters and so on. </br></br>
We train and test these three nets on MNIST data and measure the accuracy on the test set. We have set the 
number of parameters N to roughly 100000 and number of layers L to 10. For simplicity, we set the number 
of neurons in the first hidden layer to 50 for all the three cases. We use batch normalization and 
dropout (with 0.3). We also use adam optimizer with learning rate 0.0001. Furtheer we use Xavier initialization. We also use 
RELU activation and in the last layer we use softmax. Here the error function is cross entropy. </br></br>
The `output.txt` file contains the accuracy values for all three nets. </br></br>
- **The second part involves implementing (from scratch) a Neural Network and training it using backpropagation algorithm.** </br></br>
Here we implement backpropagation from scratch and use it to train a fully connected neural net with 
mini-batch vanilla gradient descent. We test our implementation on MNIST data. To check 
correctness of our implementation, we also implement the same net using standard libraries and 
train with the exactly same settings. </br></br>
The `output.txt` file contains the accuracy of the above two implementations on MNIST 
data.
