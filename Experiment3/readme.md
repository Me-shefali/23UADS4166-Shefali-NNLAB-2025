# 3-Layer NN using Tensorflow

## Objective:
Write a Program to implement a three-layer neural network using Tensor flow library (only, no keras) to classify MNIST handwritten digits dataset. Demonstrate the implementation of feed-forward and back-propagation approaches.

## Description of the model:
This program implements a three-layer fully connected neural network using TensorFlow (without Keras) to classify the MNIST handwritten digits dataset. The model follows a feed-forward neural network architecture with backpropagation for training.
-	Input layer (784 neurons), the input consists of 28x28 grayscale images.
-	Hidden layer 1 (128 neurons).
-	Hidden layer 2 (64 neurons).
-	Output layer ( 10 neurons), gives output of numbers between 0-9.
Tensorflow - TensorFlow is an open-source machine learning and deep learning library developed by Google. It is widely used for building neural networks and training AI models efficiently.
ReLU is used as an activation function.


## Description of the code:
-	Importing the libraries (numpy and tensorflow)
-	Importing the MNIST dataset which contains images of handwritten numbers.
-	Data is reshaped (28x28 matrix in the 1D vector of size 784), normalizing pixel values (0-255 to 0-1), and encoding (one-hot encoding).
-	Network parameters like the number of neurons in each layer, learning rate, epochs, and batch size are defined.
-	Weights and biases are defined for each layer (W = list of each layer’s weights , B = list of each layer’s biases).
-	Froward propagation function to find output of each layer:
              Zi = Wi.X + Bi
-	Loss function calculates the difference between predicted and actual values.
-	Backpropagation is used for updating weights.
-	Finally the model is trained and evaluated.


## Output:
      Epoch 1, Loss: 2.2877
      Epoch 2, Loss: 2.2343
      Epoch 3, Loss: 2.1234
      Epoch 4, Loss: 1.9871
      Epoch 5, Loss: 1.8813
      Epoch 6, Loss: 1.8269
      Epoch 7, Loss: 1.7605
      Epoch 8, Loss: 1.6965
      Epoch 9, Loss: 1.6628
      Epoch 10, Loss: 1.6416
      Epoch 11, Loss: 1.6268
      Epoch 12, Loss: 1.6157
      Epoch 13, Loss: 1.6071
      Epoch 14, Loss: 1.6002
      Epoch 15, Loss: 1.5945
      Epoch 16, Loss: 1.5896
      Epoch 17, Loss: 1.5855
      Epoch 18, Loss: 1.5819
      Epoch 19, Loss: 1.5788
      Epoch 20, Loss: 1.5760
      Test Accuracy: 90.98%


## Performance:
-	The accuracy of the model is 90%.
-	The loss reduces over the 20 epochs.


## My comments:
-	The model achieved high classification accuracy.
-	It uses a simple three-layer Neural Network with a ReLU activation function.
-	It has fully connected layers, requires more parameters, making it less effective and, more memory-intensive.
