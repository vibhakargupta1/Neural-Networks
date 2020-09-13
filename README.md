# Neural-Networks
This repository contains the codes/ jupyter notebooks for various neural networks developed from scratch which can be used for learning purposes if you're a beginner.
Codes in this repository can give you a basic intuition of how the Neural Networks are trained and tested. Some basic bitwise functions are implemented using neural networks for better understanding of the concepts.
The implementation examples are kept as logic functions to understand the basics of the networks properly.
## Basic Terminologies
y_in = net input to neuron ( calculated as y_in = ∑(i = 1 to n)(x_i * w_i) + b) <br/>
t = target values in training sets <br/>
y = Output after applying activation function over net input
## Activation Functions
Activation functions are the functions applied to net inputs to neurons to obtain the desired outpur from the neuron.<br/>
There are several predefined activation functions but you may create your own according to the needs or use the predefined one's.<br/>
#### Some basic activation functions:
1. [ Sigmoid function ](https://mathworld.wolfram.com/SigmoidFunction.html)
2. [ Relu Function ](https://www.wolframalpha.com/input/?i=Relu+function&x=0&y=0)
3. [ Binary step function ](https://www.analyticssteps.com/blogs/7-types-activation-functions-neural-network)
4. [ Linear ](https://www.analyticssteps.com/blogs/7-types-activation-functions-neural-network)
5. [ Leaky Relu ](https://www.analyticssteps.com/blogs/7-types-activation-functions-neural-network)
6. [ Tanh function ](https://www.analyticssteps.com/blogs/7-types-activation-functions-neural-network)
7. [ Softmax function ](https://www.analyticssteps.com/blogs/7-types-activation-functions-neural-network)

## 1. Perceptron Networks
These networks belong to supervised learning type networks. \
These networks consists of three layers. 
1. Sensory Unit (input units)
2. Associator Unit (hidden units/layers) 
3. Response Unit (Output units/layers) 

Perceptron networks learning algorithm: 
1. Initiate weights and bias (preferably kept 0 for ease) 
2. For each training input vector x_i calculate y_in as y_in = w_i * x_i + b 
3. Apply activation function to y_in 
4. Compare y_in with target values.
5. If condition satisfied then end w_i(new) = w_i(old) 
6. Else w_i(new) = w_i(old) + alpha * t * x_i 
7. If weights don't change after iterating over all training examples then end else continue steps 2-6
