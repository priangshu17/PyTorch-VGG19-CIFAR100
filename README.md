# PyTorch-VGG19-CIFAR100

This repository contains a PyTorch implementation of the VGG-19 architecture, built entirely from scratch. The model is designed for image classification on the CIFAR-100 dataset, and the complete project is contained within a single Jupyter Notebook.

## 📝 Overview

This project serves as a clear, educational guide to implementing the VGG-19 network, a highly influential deep convolutional neural network known for its simplicity and depth. The code walks through every step of the process, from data preparation to final evaluation.

### Key Features:
* **VGG-19 Architecture from Scratch**: The model is constructed using sequential blocks of 3x3 convolutional layers and max-pooling, true to the original VGG design.
* **CIFAR-100 Dataset**: The model is trained and evaluated on the CIFAR-100 dataset, which consists of 100 object classes.
* **Data Resizing**: Input images are resized to 227x227, matching the typical input dimensions for VGG-style networks.
* **Complete Training Pipeline**: The notebook includes a full pipeline for data loading, transformations, training with a validation loop, and final testing.
* **Performance Visualization**: Code is provided to plot the training and validation metrics (loss and accuracy) using `matplotlib`.

🏗️ Code Structure
The Jupyter Notebook py_vgg.ipynb is organized as follows:

Imports and Setup: Imports all necessary libraries and configures the compute device (CPU/GPU).

Data Loading & Preprocessing: Loads the CIFAR-100 dataset, applies transformations (including resizing to 227x227), and splits the data into training, validation, and test sets.

Model Definition:

The VGG19 class defines the complete network architecture. It is composed of five convolutional blocks followed by three fully-connected layers.

Training:

The model, loss function (CrossEntropyLoss), and optimizer (Adam) are initialized.

A training_loop function handles the training and validation process for each epoch.

Evaluation & Visualization:

A plot_metrics function is used to visualize the loss and accuracy curves.

The final model is evaluated on the test set to report its final accuracy.
A plot_metrics function is used to visualize the loss and accuracy curves.

The final model is evaluated on the test set to report its final accuracy.
