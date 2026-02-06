# NEURAL NETWORKS & APPLIED DEEP LEARNING – COMPLETE RANKER NOTES

## 1. What is Deep Learning?

**Deep Learning** is a subset of Machine Learning that uses **neural networks with multiple hidden layers** to learn complex patterns from data.

Hierarchy:

* Artificial Intelligence
* Machine Learning
* Deep Learning

Key idea:

> Features are **learned automatically**, not hand-crafted.

---

## 2. Biological Inspiration

Neural networks are inspired by the human brain.

Components:

* Neuron → node
* Dendrites → inputs
* Synapse → weight
* Axon → output

---

## 3. Artificial Neuron (Perceptron)

Mathematical form:
[
z = w_1x_1 + w_2x_2 + \dots + b
]
[
y = f(z)
]

Where:

* x = inputs
* w = weights
* b = bias
* f = activation function

---

## 4. Activation Functions (VERY IMPORTANT)

### Sigmoid

[
f(x) = \frac{1}{1+e^{-x}}
]

* Output: (0,1)
* Vanishing gradient issue

### Tanh

* Output: (-1,1)
* Zero-centered

### ReLU (🔥 most used)

[
f(x) = \max(0,x)
]

* Fast
* Sparse activation

### Softmax

* Used in multi-class classification
* Outputs probabilities

---

## 5. Neural Network Architecture

* Input layer
* Hidden layers
* Output layer

Key terms:

* Depth → number of layers
* Width → number of neurons per layer

---

## 6. Forward Propagation

Process:

1. Inputs multiplied by weights
2. Bias added
3. Activation applied
4. Output generated

This is **prediction phase**.

---

## 7. Loss / Cost Functions

Measure how wrong the prediction is.

### Common Loss Functions

* Mean Squared Error (Regression)
* Binary Cross-Entropy
* Categorical Cross-Entropy

Goal:

> Minimize loss

---

## 8. Backpropagation (CORE CONCEPT)

Algorithm to update weights using **gradient descent**.

Steps:

1. Compute loss
2. Compute gradients
3. Update weights

Chain rule is the backbone.

---

## 9. Gradient Descent Variants

* Batch Gradient Descent
* Stochastic Gradient Descent (SGD)
* Mini-batch Gradient Descent

Enhancements:

* Momentum
* RMSProp
* Adam (🔥 most popular)

---

## 10. Learning Rate (CRITICAL)

* Too high → divergence
* Too low → slow learning

Often tuned experimentally.

---

## 11. Overfitting & Underfitting

* **Overfitting**: good training, poor testing
* **Underfitting**: poor both

Solutions:

* Regularization
* Dropout
* More data
* Early stopping

---

## 12. Regularization Techniques

### L1 Regularization

* Encourages sparsity

### L2 Regularization

* Penalizes large weights

### Dropout

* Randomly drops neurons during training

---

## 13. Weight Initialization

* Random initialization
* Xavier initialization
* He initialization (ReLU)

Prevents vanishing/exploding gradients.

---

## 14. Vanishing & Exploding Gradients

* Vanishing → gradients go to zero
* Exploding → gradients blow up

Solutions:

* ReLU
* Proper initialization
* Batch normalization

---

## 15. Batch Normalization

* Normalizes layer inputs
* Faster convergence
* Acts as regularizer

---

## 16. Types of Neural Networks

### Feedforward Neural Network

* Basic structure

### Convolutional Neural Network (CNN)

* Image data
* Convolution + pooling

### Recurrent Neural Network (RNN)

* Sequential data

### LSTM / GRU

* Solve long-term dependency

---

## 17. Convolutional Neural Networks (CNN)

Key components:

* Convolution layer
* Pooling layer
* Fully connected layer

Applications:

* Image classification
* Object detection
  n

---

## 18. Recurrent Neural Networks (RNN)

* Handles time series
* Uses hidden state

Limitation:

* Vanishing gradients

---

## 19. Transfer Learning (APPLIED EDGE)

* Use pre-trained models
* Fine-tune for new task

Advantages:

* Less data needed
* Faster training

---

## 20. Evaluation Metrics

### Classification

* Accuracy
* Precision
* Recall
* F1-score

### Regression

* MSE
* RMSE
* R²

---

## 21. Model Deployment (Applied)

Steps:

* Save model
* Load model
* Integrate into application

---

## 22. Ethical & Practical Issues

* Bias
* Interpretability
* Energy consumption

---

## 23. Exam Traps (VERY IMPORTANT)

❌ Confusing activation vs loss
❌ Ignoring learning rate
❌ Assuming deeper = always better
❌ Forgetting overfitting controls

---

## 24. One-Page Ultra-Revision Sheet

* Neuron = weighted sum + activation
* Backprop = gradient descent + chain rule
* ReLU + Adam = default choice
* Regularization fights overfitting
* CNN → images | RNN → sequences


