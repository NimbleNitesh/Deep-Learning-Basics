# Image Age Classification using Vanilla CNN with PyTorch

This project implements a Convolutional Neural Network (CNN) from scratch using PyTorch to classify the age of individuals from images. The dataset consists of images representing 11 age groups ranging from 20 to 30 years.

## Dataset Description

The dataset comprises images grouped by age categories, with each category representing a specific age group. Images are preprocessed and resized to 128x128 pixels to ensure consistency in input dimensions for the model.

## Model Architecture: AlexNet Variant

The CNN architecture employed in this project is a variant of AlexNet. It consists of several convolutional layers followed by max-pooling layers and fully connected layers. The model architecture is defined as follows:

- Convolutional Layer 1: 64 filters, kernel size 11x11, stride 4, padding 58
- Max Pooling Layer 1: kernel size 3x3, stride 2
- Convolutional Layer 2: 192 filters, kernel size 5x5, stride 1, padding 2
- Max Pooling Layer 2: kernel size 3x3, stride 2
- Convolutional Layer 3: 384 filters, kernel size 3x3, stride 1, padding 1
- Convolutional Layer 4: 256 filters, kernel size 3x3, stride 1, padding 1
- Convolutional Layer 5: 256 filters, kernel size 3x3, stride 1, padding 1
- Max Pooling Layer 3: kernel size 3x3, stride 2
- Fully Connected Layers: 3 linear layers with ReLU activation

## Training and Evaluation

The model is trained using the Adam optimizer with a learning rate of 10. Training is conducted for 10 epochs, with early stopping implemented to prevent overfitting. During training, both training and validation losses are monitored to assess model performance.

## Prediction

Once trained, the model is used to predict the age of individuals in unseen images from a separate test dataset. Predicted ages are calculated and appended to the test dataset for further analysis.

---

This README provides an overview of the project, including dataset description, model architecture, training and evaluation process, and prediction outcomes. For detailed implementation and code explanation, refer to the corresponding Jupyter Notebook.