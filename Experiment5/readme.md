# Objective
WAP to train and evaluate a convolutional neural network using Keras Library to classify MNIST fashion dataset. Demonstrate the effect of filter size, regularization, batch size and optimization algorithm on model performance.

## Decription 
- This model is a Convolutional Neural Network (CNN) built using the Keras library.
- It is trained on the Fashion MNIST dataset, which contains 28x28 grayscale images of clothing items.
- The architecture includes two convolutional layers with max pooling, followed by a dense hidden layer and a softmax output layer.
- The model uses L2 regularization to reduce overfitting by penalizing large weights.
- Different filter sizes (3x3 and 5x5) are tested to observe their effect on feature extraction.
- It also compares various optimizers (Adam, SGD) and batch sizes (32, 64) to evaluate training efficiency and accuracy.
- The model is trained for 5 epochs with validation accuracy recorded at each step.
- A combined graph is plotted to visually analyze the effect of these hyperparameters on validation accuracy.

## Description of code
- Loads the Fashion MNIST dataset, which has images of clothes like shirts, shoes, and bags.
- Normalizes the image data so the pixel values are between 0 and 1.
- Defines a CNN model using layers like Conv2D, MaxPooling, Flatten, and Dense for image classification.
- Adds L2 regularization to prevent overfitting and make the model generalize better.
- Trains the model using different combinations of filter sizes, regularization values, batch sizes, and optimizers.
- Stores the training history (like accuracy for each epoch) for each combination.
- Evaluates the model on test data to check how well it performs.
- Plots a graph to compare the validation accuracy of each configuration across 5 training epochs.

## Output


## My comments
- The model is trained for only 5 epochs, which may not be enough for best performance.
- It uses only two convolutional layers, which might limit its ability to learn complex patterns.
- Only a few hyperparameter combinations are tested — more variations could give better insights.
- The model doesn't use data augmentation, which could help improve generalization.
- Performance could be boosted by trying deeper architectures or using dropout layers.
