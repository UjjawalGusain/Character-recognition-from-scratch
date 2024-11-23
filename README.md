
# MNIST Handwritten Digit Classification

This project focuses on the classification of handwritten digits from the MNIST dataset. It explores three different approaches to model development, ranging from building an Artificial Neural Network (ANN) from scratch to implementing pre-designed architectures such as LeNet.


## Contents

- Overview
- Dataset
- Project Workflow
- Models Developed
    - ANN from Scratch
    - ANN with Keras
    - LeNet
- Results
- Installation
- Usage
- Acknowledgments
- Future Improvements



## Descripion

The goal of this project was to classify handwritten digits (0–9) from the MNIST dataset with increasing accuracy using three approaches:

- A custom ANN implemented from scratch in Python using NumPy.
- A model built with Keras.
- A convolutional neural network (LeNet).



## Dataset

The MNIST dataset is a benchmark dataset for digit classification. It contains:

- Training Set: 60,000 grayscale images (28x28 pixels each).
- Test Set: 10,000 grayscale images.
- Each image corresponds to a label (0–9), representing the digit it depicts.


## Architecture

### 1. ANN from Scratch
- Architecture:
    - Input Layer: 784 neurons (28x28 flattened image).
    - Hidden Layer: 128 neurons with ReLU activation.
    - Output Layer: 10 neurons with Softmax activation.
    #### Key Features:
    - Implemented forward and backpropagation manually.
    - Optimized weights using stochastic gradient descent.
    - Accuracy: 95%

### 2. ANN with Keras
- Architecture:
    - Input Layer: 784 neurons (28x28 flattened image).
    - Hidden Layers: 2 dense layers with 128 and 64 neurons, both with ReLU activation.
    - Output Layer: 10 neurons with Softmax activation.
    #### Key Features:
    - Built with Keras, utilizing its high-level API for easy implementation.
    - Trained using the Adam optimizer and categorical cross-entropy loss.
    - Accuracy: 97.66%
#### 3. LeNet (Convolutional Neural Network)
- Architecture:
    - Convolutional layers followed by max-pooling layers.
    - Fully connected layers for classification.
    #### Key Features:
    - Implemented a CNN model inspired by Yann LeCun's LeNet architecture.
    - Leveraged convolutional layers for feature extraction.
    - Accuracy: 98.24%


## Accuracy Summary

Model  | Test Accuracy |
------------- | ------------- |
ANN from scratch  | 95%  |
ANN using Keras | 97.66%  |
LeNet Architecture  | 98.24%  |


~ `Inspired by the simplicity of implementing neural networks from scratch and leveraging modern libraries like Keras for complex architectures.`
