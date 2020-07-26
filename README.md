# Neural Network Basics
Primer to understanding neural networks using numpy for applications in classification and regression, and comparing with non-linear logistic and non-linear regression for the same. Datasets for [classification](https://www.kaggle.com/zaurbegiev/my-dataset) (modeling loan status) and [regression](https://www.kaggle.com/shivachandel/kc-house-data) (modeling house prices) taken from Kaggle.

Some concepts covered in this repository include:
1. Cross-validation: Cross validation is the method of dividing up the training data into a certain number of folds, and then train on different folds to see which fold can give the best training and validation accuracies for prediction. For 5-fold cross validation, we would divide the data into 5 sets, use the first 1 for testing, next 1 for validation, and last 3 for training. Then we would shuffle or rotate between these sets. Cross validaton allows us to choose the best parameters that learn best from the given training data while not being underfitted or overfitted.
2. Neural networks for regression: Neural networks are computational models for prediction based on the neural synaptic connections observed in the human brain. They consist of individual units called neurons, which are similar to perceptrons in their computational function, and similar to human neurons in the principle with which they work. These units are arranged into layers, modeled behind the functioning of the brain forming synaptic connections. The basic structure of a neural network includes an input layer, one or more hidden layers, and an output layer. The input layer takes in the inputs, and the output layer sends out the predictions made by the neural network. The hidden layer(s) consists of multiple neurons working together to compute representations that can allow the neural network to compute predictions for the output.
3. Neural networks for classification: Nonlinear logistic regression using neural networks models nonlinear relations in the data and uses logistic regression to provide predictions. To emulate the NeuralNet class and update it for NeuralNetLogReg, we use the indicator target labels for training to update the weights for the linear model. For the error function, we can derive the gradient by switching the squared error with the negative log likelihood function. We use the softmax of the probabilities for the classes generated by the neural network to get classification results.