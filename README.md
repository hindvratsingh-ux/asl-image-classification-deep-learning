# American Sign Language Image Classification

## Overview
This project explores deep learning approaches for classifying American Sign Language (ASL) hand-sign images. It compares three model families: a custom Convolutional Neural Network (CNN), a transfer learning approach based on ResNet-50, and a Vision Transformer (ViT).

## Objective
The goal of this project was to build and compare image classification models for recognizing ASL alphabet gestures and to evaluate the trade-offs between predictive performance, computational efficiency, and training complexity.

## Dataset
The models were trained and evaluated using the Kaggle ASL Alphabet dataset, which contains 29 hand-sign classes. The data includes real-world variation in lighting, background, hand shape, skin tone, and camera angle, making it suitable for robust visual classification experiments.

## Models Implemented
- Custom CNN trained from scratch
- ResNet-50 transfer learning model
- Vision Transformer (ViT-Tiny)

## Tools and Frameworks
- Python
- TensorFlow / Keras
- PyTorch
- timm
- NumPy
- Matplotlib / evaluation utilities

## Methodology

### 1. Data preparation
The dataset was preprocessed and split into training, validation, and test sets. Data augmentation techniques such as random rotation, horizontal flipping, and brightness/contrast changes were used to improve generalization in training.

### 2. Custom CNN
A baseline CNN was built to learn ASL features directly from images. This model provided a lightweight benchmark for comparison against more advanced pretrained architectures.

### 3. Transfer Learning
A pretrained ResNet-50 model was adapted for ASL classification using a two-phase strategy:
- feature extraction with frozen backbone layers
- fine-tuning of higher-level layers for task-specific adaptation

### 4. Vision Transformer
A pretrained Vision Transformer model was fine-tuned for 29-class ASL classification. This model used patch-based image representations and self-attention to capture global relationships between image regions.

### 5. Comparative evaluation
The three models were compared using classification accuracy, loss behaviour, confusion matrices, and training efficiency to understand the trade-offs between speed, complexity, and predictive performance.

## Key Findings
- The custom CNN provided strong baseline performance with fast training and low computational cost.
- The ResNet-50 transfer learning model achieved the highest overall accuracy but required the most training time and computational resources.
- The Vision Transformer delivered very high accuracy with a better balance between performance and efficiency than full transfer learning.
- The project showed that pretrained deep learning models significantly improve ASL image classification performance compared with a baseline CNN trained from scratch.


## Applications
This project is relevant to:
- computer vision
- image classification
- assistive technology
- gesture recognition
- human-computer interaction


## Summary
This project demonstrates practical experience in deep learning, transfer learning, transformer-based vision models, comparative model evaluation, and image-based classification using real-world data.
