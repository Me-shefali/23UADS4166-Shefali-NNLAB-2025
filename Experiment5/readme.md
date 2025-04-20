# Objective
WAP to train and evaluate a convolutional neural network using Keras Library to classify MNIST fashion dataset. Demonstrate the effect of filter size, regularization, batch size and optimization algorithm on model performance.

## Description 
- This model is based on the ResNet18 architecture, a deep convolutional neural network pretrained on the ImageNet dataset.
- It leverages transfer learning by reusing learned features from ImageNet to classify medical images.
- The final fully connected (FC) layer of the model is replaced to match the number of target medical classes.
- The input images are resized to 224x224 pixels and normalized to match ImageNet standards.
- The model is fine-tuned using the CrossEntropyLoss function and the Adam optimizer.
- It is trained over several epochs using a batch size of 32, adjusting the weights to minimize classification error.
- Performance is validated on a separate dataset using accuracy as the evaluation metric.
- Once trained, the model can accurately classify new, unseen medical images into their respective categories.

## Description of code
- It checks if a GPU is available to speed up training (if not, it uses the CPU).
- It loads a pretrained ResNet18 model, which has already learned how to detect general image features.
- The last layer of the model is changed to match the number of classes in your medical image dataset.
- Your image dataset is loaded using a folder structure where each folder name represents a class (like “X-rays” or “MRIs”).
- Image transformations (like resizing, flipping, and normalizing) are applied to make all images suitable for training.
- The model is then trained for several rounds (epochs) by showing it batches of images and adjusting it based on errors.
- It checks the model’s accuracy on a separate validation set after each round.
- Finally, the trained model is saved so it can be used later to classify new medical images.
 
## My comments
- The model might not perform well if the medical dataset is too small or imbalanced.
- It uses basic data augmentation — adding more advanced techniques could improve accuracy.
- Only the last layer is fine-tuned — training more layers could help the model learn better.
- The model is based on ResNet18, which is small — trying deeper models like ResNet50 may give better results.
- Validation accuracy alone may not be enough — adding metrics like precision and recall can give deeper insights.
  
