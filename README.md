# Neural_Network_Charity_Analysis

## Analysis Overview 

The purpose of this analysis is to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

## Deliverables:
This assignment consists of 3 technical analysis deliverables and a written report on the Credit Risk Analysis. 

1. ***Deliverable 1:*** Preprocessing Data for a Neural Network Model
2. ***Deliverable 2:*** Compile, Train, and Evaluate the Model
3. ***Deliverable 3:*** Optimize the Model
4. ***Deliverable 4:*** A Written Report on the Neural Network Model (README.md)

## Results

### Data Preprocessing 

- What variable(s) are considered the target(s) for your model? ***IS_SUCCESSFUL column***

- What variable(s) are considered to be the features for your model? ***Every column except the IS_SUCCESSFUL column***

- What variable(s) are neither targets nor features, and should be removed from the input data? ***EIN and NAME columns***

### Compiling, Training and Evaluating the Model

#### How many neurons, layers, and activation functions did you select for your neural network model and why? 

- My neural network had 2 hidden layers: layer1 at 80 neurons and layer2 at 30 neurons 
-To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.

#### Were you able to achieve the target model performance?

- The model accuracy is under 75% at 70.9%. 

#### What steps did you take to try and increase model performance?

- To increase the performance of the model I removed the USE_CASE column

![USE_CASE.png](/Results/USE_CASE_accuracy.png)

- This caused the accuracy to decrease to 56.5%

![USE_CASE_accuracy.png](/Results/USE_CASE_accuracy.png)

- Increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.

![additional_layer_neurons.png](/Results/additional_layer_neurons.png)

- This resulted in a lower accuracy score than the original 70.9% accuracy. 

![additional_layer_neurons_accuracy.png](/Results/additional_layer_neurons_accuracy.png)

- I also tried a different activation function (tanh) with the original hidden layers and neurons. 

![tanh.png](/Results/tanh.png)

- This resulted in an even lower accuracy score than the second attempt. 

![tanh_accuracy.png](/Results/tanh_accuracy.png)



## Summary
