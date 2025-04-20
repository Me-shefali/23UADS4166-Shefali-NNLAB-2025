# RNN 

## Objective
Write a Program to train and evaluate a Recurrent Neural Network using PyTorch Library to predict the next value in a sample time series dataset. 

## Description of model
- Input Layer:
    - Accepts sequences of time series data with a fixed length (e.g., 20 consecutive time steps).
    - Each input is a 1-dimensional value (since we're using a single sine wave signal).
- RNN Layer:
  - The core of the model.
  - This layer processes the input sequence step by step.
  - It has:
    - Input size: 1 (one value per time step)
    - Hidden size: A hyperparameter (e.g., 50) that defines how many neurons the RNN uses to store information.
    - Number of layers: Determines how many stacked RNN layers the model has (usually 1 or 2 in basic setups).
  - The RNN maintains a hidden state, which is updated at each time step. This allows the model to capture temporal dependencies in the sequence.
- Fully Connected (Linear) Output Layer:
  - After the RNN processes the entire sequence, only the final hidden state (from the last time step) is passed to this layer.
  - This layer converts the final hidden representation into a single output value: the predicted next point in the time series.

## Description of code
- Import libraries ( PyTorch, NN, numpy, matplotlib)
- Generated the sine wave to work on.
- Splits the sine wave into: Input sequences of length seq_length, Target values: the next value after the sequence.
- Intializing the hyperparameters.
- Preparing the data for training: 80% training and 20% testing data.
- Defining the RNN nodel.
- Finding the loss(Loss function: Mean Squared Error for regression) and applying the optimizer(Optimizer: Adam for training efficiency).
- Finally the model is trained and evaluated.
- Ploting the graph to compare the actual and predicted output.

## Output
    Epoch [10/100], Loss: 0.0258
    Epoch [20/100], Loss: 0.0061
    Epoch [30/100], Loss: 0.0026
    Epoch [40/100], Loss: 0.0001
    Epoch [50/100], Loss: 0.0002
    Epoch [60/100], Loss: 0.0001
    Epoch [70/100], Loss: 0.0000
    Epoch [80/100], Loss: 0.0000
    Epoch [90/100], Loss: 0.0000
    Epoch [100/100], Loss: 0.0000

## My comments
- RNNs forget long-term patterns easily.
- They may lag or miss sharp changes in data.
- Not ideal for complex or noisy time series.
- Can be improved by using LSTM or GRU.
- Better tuning and more layers can boost accuracy.
