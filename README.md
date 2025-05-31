# Alzheimers Classifier

This project uses machine learning to classify brain MRI images for early detection of Alzheimer's disease. It is designed to assist in medical diagnostics by identifying patterns associated with various stages of cognitive decline.

## Project Overview

Alzheimer’s Disease (AD) affects millions globally, and early detection is key to managing its progression. This project builds a model to classify MRI images into stages of Alzheimer's, using deep learning for pattern recognition.

## Features

# AI Agent
- Classification of MRI brain scans into:
  - **Non-Demented**
  - **Mildly Demented**
  - **Moderately Demented**
  - **Very Mildly Demented**
- Uses CNN (Convolutional Neural Networks) for image classification
- Training and evaluation with clean visualization of model accuracy and loss
- Dataset preprocessing and augmentation to improve generalization
- Transfer learning via the pre-trained EfficientNetb0 CNN for data constraints
- Trained via PyTorch and Cuda

## Web Application

This project includes a fully responsive Bootstrap-powered website that provides an educational and interactive experience around Alzheimer's detection. It is designed to both inform users about Alzheimer's disease and showcase the image classification model in action.

# Features
  - Homepage: Welcomes users with a mission statement and navigation to key sections.
  - Classifier Page: Allows users to upload MRI images and receive AI-based predictions (assuming integration with backend).
  - Educational Content: Offers external articles and Alzheimer’s-related resources.
  - About Us: Provides background on the team and the motivation behind the project.

# Integration

The trained AI model path was integrated into the website classifier via FastAPI. The website was briefly hosted in December 2024 via Amazon Web Service


## Dataset

The dataset used is from Kaggle, uploaded by Aryan Singhal:

- Format: JPEG or PNG MRI images
- Labels: NonDemented, MildDemented, ModerateDemented, VeryMildDemented
- Preprocessed for normalization and resizing

> Dataset source: https://www.kaggle.com/datasets/aryansinghal10/alzheimers-multiclass-dataset-equal-and-augmented


## Performance

  - 98.44% model testing accuracy.
  - Achieved in under 15 epochs
  - Precision, recall, and f1-scores nearly perfect (>=.98)
  - Performs equally with minimal disparities between all four classes
  - Performs equally well on the OASIS dataset


# AI Tech Stack
  - Torch, Cuda
  - Scikit-Learn
  - EfficientNetb0
  - ResNet50
  - FastApi




