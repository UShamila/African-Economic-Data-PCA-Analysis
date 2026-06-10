# African Economic Data PCA Analysis

## Overview

This project implements Principal Component Analysis (PCA) from scratch using NumPy on African economic indicators (1980–2022). The goal is to reduce dataset dimensionality while preserving maximum variance using core linear algebra concepts (covariance, eigenvalues, and eigenvectors).

---

## Objectives

* Clean and preprocess African economic dataset
* Handle missing values (NaN) and non-numeric columns
* Standardize data using z-score normalization
* Compute covariance matrix manually
* Perform eigendecomposition (eigenvalues & eigenvectors)
* Sort principal components by explained variance
* Project data onto lower-dimensional space
* Visualize data before and after PCA
* Select optimal components using explained variance tradeoff

---

## Methodology

PCA was implemented manually without machine learning libraries.

### 1. Standardization

[
z = \frac{x - \mu}{\sigma}
]

### 2. Covariance Matrix

Computed using NumPy to measure relationships between features.

### 3. Eigendecomposition

Extracted eigenvalues and eigenvectors to identify principal components.

### 4. Dimensionality Reduction

Projected standardized data onto top-k eigenvectors.

### 5. Explained Variance

Eigenvalues were used to determine how much information each component retains.

---

## Tradeoffs

Reducing dimensions improves efficiency and simplifies the dataset but:

* Reduces interpretability of original features
* May lose subtle relationships between economic indicators (GDP, inflation, unemployment)

---

## Dataset

* African Economic Indicators (1980–2022)
* 7+ features
* Contains missing values and non-numeric columns handled during preprocessing

---

## Tools Used

* Python
* NumPy
* Pandas
* Matplotlib

---

## Outcome

The dataset was successfully reduced into principal components while preserving major variance patterns for analysis and visualization.

