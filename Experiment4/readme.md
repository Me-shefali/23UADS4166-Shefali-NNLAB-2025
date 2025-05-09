# Different configuration of hidden layer and learning rate

## Objective:
Write a program to evaluate the performance of implemented three-layer neural network with variations in activation functions, size of hidden layer, learning rate, batch size and number of epochs


## Description of the model:
This code implements a fully connected neural network (feedforward neural network) using TensorFlow to classify handwritten digits from the MNIST dataset.
-    Structure : Input layer (784 neurons), two hidden layer [(160,100),(100,100)..etc.] and one output layer.
-    Activation function used in hidden layers are ReLU (Rectified Linear Unit).
-    Loss function used in this code is Softmax cross-entropy.
-    Learning rate used are [0.01, 0.1, 1].
This model iterates through the different combinations of hidden layers and learning rates to find the differnce between performances under different conditions. This loop runs for 15 different combinations and calculates loss and accuracy for each epoch and plots a graph for each combination of easy comparisions.


## Description of the code:
-    Importing the necessary libraries.
-    Loads the MNIST dataset, reshapes the images, normalize the pixel values of image and finally performs one hot encoding for multiclass classification.
-    Defining the parameters (input layer, hidden layers, batch size, number of epochs, learning rate).
-    Iterating through different model configurations.
-    Assigning weights and biases to the layers.
-    Performing the actions on the layers using activation function.
-    Calculating loss and accuracy each time.
-    After the complition of epochs, calculates the execution time of loop, plotting a graph of loss and accuracy, plot confusion matrix.


## Performance:
-    This code succesfully calculates the loss and accuracy of each configuration.


## My Comments:
-    The model does not perform well when learning rate is more (for example 1), it does not reduces the loss much which affects the training process.
-    Learning rates: 0.01 and 0.1, the accuracy is nearly same and the results are also similar, the only differnce is execution time: in most of the cases when learning rate is 0.01 it takes less time to execute in comparision when learning rate is 0.1 .
-    When LR is 0.01 the accuracy smoothly increases and loss smoothly decreases while when LR is 0.1 the results fluctuates more.
-    Hidden layer does not effect much in this case.
-    Limitations: MLP is not best for image classification, using CNN is better option.
