# MNIST Hidden Layer Representation Study

## Overview

This project investigates how hidden-layer size influences both performance and interpretability in a single-hidden-layer dense neural network trained on the MNIST dataset.

Rather than focusing only on accuracy, this study examines how internal representations evolve as model capacity increases. By systematically varying the number of hidden neurons, the project reveals how neural networks transition from underfitting to effective generalization and how learned feature spaces become more structured.

## Dataset

* **Dataset:** MNIST handwritten digits
* **Training samples:** 60,000
* **Test samples:** 10,000
* **Image size:** 28 × 28 (flattened to 784 features)
* **Classes:** 10 digits (0–9)

All inputs were normalized to the range [0, 1].

## Objective

To understand how increasing hidden-layer width affects:

* Classification accuracy
* Feature space separability
* Interpretability of learned representations

## Experimental Design

All models share the same architecture except for hidden-layer size:

* Input layer: 784 features
* Hidden layer: variable (1, 2, 3, 5, 20, 50, 85 neurons)
* Activation: ReLU
* Output layer: Softmax (10 classes)
* Training: Backpropagation

Evaluation methods include:

* Training, validation, and test accuracy
* Loss curves
* Confusion matrices
* Hidden-layer activation visualizations
* Misclassified digit inspection

## Key Experiments

### 1. Hidden Layer Scaling

Models were trained with increasing hidden neurons to observe:

* Underfitting a
