# Dermatology Image Classification with Noisy Labels

## Problem Statement
This project addresses a real-world dermatology image classification task where
training labels may be noisy, while validation data is clean and expert-verified.

## Dataset
- Image size: 28×28 (RGB)
- Number of classes: 7
- Training labels: Noisy
- Validation labels: Clean

## Approach
- Lightweight but robust CNN architecture
- Regularization using Dropout and Batch Normalization
- Validation-driven training using EarlyStopping
- Avoided aggressive resampling due to noisy labels
  
## Results
- Training accuracy is lower due to noisy annotations
- Validation accuracy is significantly higher, indicating good generalization

## Inference
A utility function is provided to load a new dataset and evaluate accuracy,
which can be used during live evaluation.
