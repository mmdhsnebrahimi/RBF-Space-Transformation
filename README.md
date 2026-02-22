# Artificial Neural Networks: RBF Space Transformation 🌌🧠

## Overview
This repository contains an analytical Artificial Neural Networks project focused on feature space transformation. The primary objective is to demonstrate how non-linearly separable data in a low-dimensional space can become linearly separable when mapped to a higher-dimensional space using Radial Basis Functions (RBF).

## The Core Concept
The project takes a complex 2D dataset where the classes cannot be separated by a simple straight line. Instead of building a deep, complex network, the code elegantly maps these 2D data points into a new, higher-dimensional feature space. The coordinates in this new space are defined by the outputs of multiple Gaussian RBF centers.

## Key Features & Workflow
* **RBF Feature Mapping:** Transforming original 2D coordinates (`X_2d`) into an expanded RBF space utilizing carefully positioned centers and optimized Sigma values.
* **Linear Classification Test:** Employing a basic Linear Classifier (`LogisticRegression`) to explicitly prove that the data has become linearly separable in the new RBF space.
* **Performance Comparison:** Rigorously comparing the classification accuracy of the linear model on two distinct fronts:
  1. The original 2D feature space (yielding low accuracy due to non-linearity).
  2. The newly constructed RBF feature space (yielding significantly improved accuracy).
* **Mathematical Verification:** Practically validating Cover's Theorem on the separability of patterns.

## Technologies Used
* **Python 3**
* **Jupyter Notebook**
* **NumPy** (For core mathematical transformations and RBF calculations)
* **Scikit-Learn** (Utilizing `LogisticRegression` and `accuracy_score` for comparative analysis)
