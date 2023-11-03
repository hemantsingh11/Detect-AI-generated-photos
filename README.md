﻿# Detect-AI-generated-photos

 
## Overview
This project aims to detect AI-generated fake images using machine learning techniques. The dataset consists of flattened 20x20 images with 1200 features.

## Installation
The project requires Python 3 and the following libraries:

- Numpy
- Pandas
- TensorFlow
- Keras
- Scikit-learn
- Imblearn
- Matplotlib
- XGBoost


## Data
The dataset contains 3850 real images and 1400 fake images generated by AI. The data is imbalanced with more real images. The images are preprocessed and flattened into 1200 features.

## Models
Several machine learning models were explored:

- Multilayer Perceptron (MLP)
- Convolutional Neural Networks (CNNs)
- Transformers
- XGBoost
- K-Nearest Neighbors (KNN)
- Random Forests
- Support Vector Machines (SVMs)
- Naive Bayes
- Ensembles of the above models

The best performing model was a stacking ensemble with KNN, Logistic Regression, XGBoost as base learners and Gaussian Naive Bayes as the meta learner. This model achieved the highest Bitgrit score of 0.95988 on the test set.

## Usage
The Jupyter notebook `source_code_colab_notebook.ipynb` contains the full machine learning pipeline including data preparation, model training, evaluation, and predictions.

