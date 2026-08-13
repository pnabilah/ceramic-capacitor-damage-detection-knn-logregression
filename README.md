# Ceramic Capacitor Damage Detection with KNN and Logistic Regression

Binary classification of multilayer ceramic capacitor (MLCC) damage using acoustic measurement features. The classification is performed using K-Nearest Neighbors (KNN) and Logistic Regression, both implemented from scratch.

This project was originally developed as a group assignment for ENEE605030 – Modeling and Machine Learning course at the University of Indonesia.

## Overview

The dataset contains acoustic measurements from 180 multilayer ceramic capacitors (MLCCs). Each sample is represented by eight acoustic features extracted from a frequency sweep, with labels indicating whether the capacitor is damaged.

The project includes:

- Data preprocessing and standardization
- Logistic Regression implemented from scratch using batch gradient descent
- KNN implemented from scratch
- Three KNN distance metrics:
  - Minkowski
  - Euclidean
  - Manhattan
- Confusion matrix and classification metrics for model evaluation
- Visualization of KNN decision boundaries

## Dataset

The dataset is the **Acoustic Measurement for Multilayer Ceramic Capacitor Damage Detection** dataset.

Each sample contains eight acoustic features:

- Maximum resonance amplitude
- Frequency of the highest resonance peak
- Amplitude of the second-highest resonance peak
- Frequency of the second-highest resonance peak
- Total phase shift
- Median amplitude of the top 10 resonance peaks
- Median frequency of the top 10 resonance peaks
- Mean group delay ripple

The target label indicates:

- `0` — No damage
- `1` — Damage

Dataset source:

- [IEEE DataPort — MLCC Acoustic Data](https://ieee-dataport.org/open-access/mlcc-acoustic-data-2220-case-size-processed)

## Methods

### Logistic Regression

Logistic Regression is implemented from scratch using:

- Sigmoid activation
- Binary cross-entropy cost
- Gradient computation
- Batch gradient descent

### K-Nearest Neighbors

KNN is implemented from scratch using three distance metrics:

- Minkowski distance
- Euclidean distance
- Manhattan distance

## Evaluation

The models are evaluated using:

- Accuracy
- Error rate
- Precision
- Recall
- Specificity
- F1 Score
- Confusion matrix

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook