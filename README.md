# SVD-based Classification of MNIST

## Overview
This project presents a machine learning approach to handwritten digit classification using linear algebraic subspace methods. Instead of deep neural networks, the method leverages Singular Value Decomposition (SVD) to model each digit class as a low-rank linear subspace.

The approach demonstrates how classical linear algebra techniques can be effectively applied to modern classification problems, providing both interpretability and strong performance.

---

## Methodology
- The MNIST dataset is used, consisting of grayscale images of handwritten digits (0–9).
- Each image is vectorized and grouped by digit class.
- For each class, a low-rank subspace is learned using truncated Singular Value Decomposition (SVD).
- Classification is performed by projecting test images onto each class-specific subspace.
- The predicted label is assigned based on the minimum projection residual.

---

## Mathematical Intuition
Singular Value Decomposition provides an orthogonal basis that captures the dominant structure of high-dimensional data. By retaining only the leading singular components, truncated SVD yields a compact representation that preserves the most important variations within each digit class.

These low-rank subspace models enable efficient and accurate classification by measuring how well a test image can be represented by each class-specific subspace.

---

## Results
The SVD-based subspace classifier achieves high classification accuracy on the MNIST test dataset (typically exceeding 95%). This highlights the effectiveness of low-rank representations for handwritten digit recognition and illustrates the power of linear algebraic methods in machine learning.

---

## Files
- `svd_mnist_classification.ipynb` — Full implementation, experiments, and visualizations

---

## Tools & Libraries
- Python
- NumPy
- SciPy
- TensorFlow
- Matplotlib

---

## Notes
This project is based on a university coursework assignment.  
All implementation, analysis, and explanations are my own.

