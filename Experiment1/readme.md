# Perceptron Learning Algorithm

## Objective:
  Write a Program to implement the Perceptron Learning Algorithm using numpy in Python. Evaluate the performance of a single perceptron for NAND and XOR truth tables as input datasets.

## Description:
  A perceptron is a single-layer neural network and the simplest artificial neural network. It consists of input nodes, weights, a bias term, and an activation function. 
    •	Weighted sum is calculated by multiplying the inputs with the weights and adding them.
    •	Activation function classifies the output using these weighted sums.
  If weighted sum >= 0, then output = 1
  If weighted sum < 0, then output = 0


## Description of code:
   1.	Class perceptron  -
        -	Initializes the weights and bias to 0.
        -	It contains an activation function that classifies the output.
        -	A predict function that predicts the output using the activation function.
        -	A train function that trains the model to find the required weights.
        -	An evaluate function that calculates the accuracy.
   2.	 Training and Evaluation for NAND Gate -
        -	The NAND truth table (nand_X) and labels (nand_y) are defined.
        -	The perceptron is trained using the train() method.
        -	The model accuracy is calculated using the evaluate() function.
        -	The predictions for all inputs in the NAND table are displayed.
   3.	Training and Evaluation for XOR Gate  -
        -	The XOR truth table (xor_X) and labels (xor_y) are defined.
        -	The perceptron is trained and evaluated on the XOR data.
        -	Accuracy is computed, and predictions for all XOR inputs are printed.

## Output:
  Training Perceptron for NAND Gate
  NAND Perceptron Accuracy: 1.0  
  Predictions for NAND Truth Table:
    Input: [0 0], Prediction: 1
    Input: [0 1], Prediction: 1
    Input: [1 0], Prediction: 1
    Input: [1 1], Prediction: 0

Training Perceptron for XOR Gate
  XOR Perceptron Accuracy: 0.5
  Predictions for XOR Truth Table:
    Input: [0 0], Prediction: 1
    Input: [0 1], Prediction: 1
    Input: [1 0], Prediction: 0
    Input: [1 1], Prediction: 0

## Performance:
NAND Gate
- Accuracy: 1.0 (100%)
- Predictions: Correct for all inputs.

 XOR Gate
- Accuracy: Approximately 0.5 (50%)
- Predictions: Incorrect for half inputs.


## My comments:
-	The perceptron cannot work properly on non-linearly separable data. Because of this, the perceptron is unable to learn the XOR gate.
-	To improve this, we can use multi-layer perceptron.




