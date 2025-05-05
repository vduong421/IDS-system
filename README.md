# Network Intrusion Detection using Machine Learning

This repository contains a Notebook (`main.ipynb`) that trains and evaluates machine learning models for detecting network-based attacks. The notebook includes data preprocessing, resampling using SMOTE, model training, evaluation, and visualization.

## Overview

The notebook performs the following steps:

1. Load and merge CSV files
2. Clean and preprocess data
3. Split the dataset using stratified train-test split
4. Apply SMOTE to handle class imbalance
5. Train and evaluate machine learning models (stock and tuned)
6. Generate confusion matrices and comparison charts

## Models Used

Each of the following models was evaluated in both stock (default) and tuned configurations:

- Random Forest
- Support Vector Machine (SVM) with RBF kernel
- Multi-layer Perceptron (MLP)

## Metrics Evaluated

For each model, the following performance metrics were calculated:

- Accuracy (overall only)
- Precision (per class and overall)
- Recall (per class and overall)
- F1 Score (per class and overall)

Note: Accuracy is reported as a single value for the entire model and is not meaningful per class.

## SMOTE Usage

SMOTE (Synthetic Minority Over-sampling Technique) is used to address class imbalance in the training set by generating synthetic samples for underrepresented classes. This helps the models generalize better across all classes.

## Visualizations

The notebook includes:

- Confusion matrices for each model
- Comparison bar charts:
  - Between stock and tuned versions of the same model
  - Across all stock models
  - Across all tuned models

## Requirements

Install required libraries using:

