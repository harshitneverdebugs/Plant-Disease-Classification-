# Plant Disease Classification using Deep Learning

This project aims to classify images of various plant diseases using a convolutional neural network (CNN). The dataset used is the New Plant Diseases Dataset, which contains augmented images of healthy and diseased plants.

## Table of Contents

- [Installation](#installation)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [Usage](#usage)
- [License](#license)

## Installation

To run this project, ensure you have the following libraries installed in your Python environment:
pip install kaggle
pip install torchsummary
pip install numpy
pip install pandas
pip install seaborn
pip install matplotlib
pip install tensorflow

##Dataset
The dataset used in this project is the New Plant Diseases Dataset, which consists of various categories of plant diseases. The dataset is organized into training, validation, and testing sets.

##Data Preprocessing
Kaggle API Authentication: Upload your kaggle.json file to authenticate and download the dataset using the Kaggle API.
Unzipping Dataset: The downloaded dataset is unzipped to extract the images and their labels.
Data Preparation: The paths to the images and their corresponding labels are stored in a DataFrame for easy access and manipulation.
Model Architecture
The model is built using Keras Sequential API and consists of:

##Multiple convolutional layers followed by max pooling layers.
A flatten layer to convert the 2D matrices to a 1D vector.
Dense layers with dropout for regularization.
Training and Evaluation
The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss function.
The model is trained for 15 epochs, and training and validation metrics are plotted for visualization.
Evaluation metrics such as accuracy, precision, and recall are calculated on the validation set, along with a confusion matrix.
Results
The results include training and validation accuracy and loss plots, confusion matrix visualizations, and precision-recall curves for each class.

##Usage
To predict the class of new images:

##Place the images in the designated test folder.
Run the prediction code to display the images along with their predicted class names and probabilities.

The training accuracy and test accuracy is 0.9717 and 0.9414 and the model is well fitted.
