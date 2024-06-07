# Vanilla Neural Network for 3-Class Classification

This repository contains a PyTorch implementation of a Vanilla Neural Network for a 3-class classification problem. The code explores different neural network architectures and optimization techniques to find the best model for the given task.

## Getting Started

### Prerequisites

- Python (>=3.6)
- PyTorch (>=1.7)
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

### Dataset

The dataset used for this problem is generated using scikit-learn's `make_moons` function. It consists of two moons, with each moon belonging to a different class. The dataset is then divided into training and testing sets.

### Neural Network Architecture

The neural network architecture used for experimentation consists of:
- Input layer with 2 inputs
- Hidden layers with ReLU activation
- Output layer with softmax activation for 3-class classification

## Training and Evaluation

The neural network is trained using various optimization techniques such as Gradient Descent, Stochastic Gradient Descent, Adam, and AdamW. Different hyperparameters like learning rate, momentum, weight decay, and dropout are also explored to improve model performance.

The training process involves iterating over the dataset for multiple epochs and updating the network parameters using backpropagation. During training, the loss is monitored, and after each epoch, the model's accuracy is evaluated on both the training and testing datasets.

## Results

The performance of each neural network configuration is evaluated based on its accuracy on the testing dataset. Contour plots are generated to visualize the decision boundaries learned by the model.