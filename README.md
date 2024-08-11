

# MNIST Digit Classification with TensorFlow

This repository contains a simple neural network model built with TensorFlow and Keras for classifying handwritten digits from the MNIST dataset.

## Table of Contents
- [Introduction](#introduction)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

## Introduction

This project demonstrates the implementation of a basic neural network for digit classification using the MNIST dataset. The model is designed to recognize handwritten digits (0-9) by learning patterns from labeled images. The dataset is a standard benchmark in machine learning and computer vision.

## Model Architecture

The neural network model consists of the following layers:

1. **Input Layer (Flatten Layer):** Converts the 28x28 pixel images into a 1D array of 784 pixels.
2. **Hidden Layer (Dense Layer):** A fully connected layer with 128 neurons and ReLU activation.
3. **Dropout Layer:** Regularizes the model by dropping out 20% of the neurons during training.
4. **Output Layer (Dense Layer):** A fully connected layer with 10 neurons and softmax activation to predict the digit class.

The model is compiled using the Adam optimizer and trained using the sparse categorical cross-entropy loss function, with accuracy as the evaluation metric.

## Dataset

The MNIST dataset consists of 60,000 training images and 10,000 testing images of handwritten digits. Each image is 28x28 pixels, grayscale, and labeled with a digit from 0 to 9.


## Results

The model achieves an accuracy of approximately **98%** on the MNIST test set after 10 epochs of training. 
Final training loss: 0.0809
Final validation loss: 0.0685
The model's loss decreased steadily during training, with the validation loss closely tracking the training loss, indicating that the model did not overfit the data.


## Acknowledgements

- The [MNIST dataset](http://yann.lecun.com/exdb/mnist/) was developed by Yann LeCun, Corinna Cortes, and Christopher J.C. Burges.
- The model was built using [TensorFlow](https://www.tensorflow.org/) and [Keras](https://keras.io/).
