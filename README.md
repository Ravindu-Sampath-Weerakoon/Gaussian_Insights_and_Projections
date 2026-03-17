# Gaussian Insights & Projections

A comprehensive exploration of the mathematical and statistical foundations of Gaussian distributions, linear algebra, and multivariate data analysis using Python.

## 🚀 Project Overview
This project provides a step-by-step walkthrough of how linear algebra concepts like eigen-decomposition and Cholesky factorization underpin the behavior of random variables and multivariate data. It covers everything from basic vector operations to the Central Limit Theorem and projected variance analysis.

## 📂 Key Phases

### Phase 1: The Linear Algebra Foundation
*   **Symmetric Matrices & Covariance:** Understanding the property $B = B^T$ and its role in data representation.
*   **Vector Operations:** Practical implementation of dot products, norms, and calculating angles between vectors.
*   **Eigen-decomposition ($B u = \lambda u$):** Identifying principal directions (eigenvectors) and variance strength (eigenvalues).
*   **Orthonormality:** Verification of the identity matrix property ($U U^T = I$) for symmetric matrices.

### Phase 2: Randomness & The Central Limit Theorem
*   **Uniform Noise:** Generating finite sample noise from uniform distributions.
*   **Gaussian Approximation:** Demonstrating the "Sum of 12" trick to transform uniform samples into a normal distribution.
*   **Estimation Uncertainty:** Visualizing how increased sample sizes improve the certainty of statistical estimates.

### Phase 3: Multi-variate Gaussian Properties
*   **Cholesky Decomposition:** Sampling from multivariate Gaussians $\mathcal{N}(m, C)$ by finding $A$ such that $AA^T = C$.
*   **Projected Variance:** Investigating how data variance shifts across different projection angles and its relationship to the covariance matrix's largest eigenvalue.

## 🛠️ Technologies & Key Tool Usage

### 📦 NumPy (Numerical Computing)
Used for high-performance linear algebra and statistical operations:
*   **`np.linalg.eig`**: To perform eigen-decomposition and extract principal components.
*   **`np.linalg.cholesky`**: To implement Cholesky Factorization for multivariate sampling.
*   **`np.dot` & `np.linalg.norm`**: For vector projections and calculating geometric properties.
*   **`np.random.rand` & `np.random.randn`**: For simulating uniform noise and standard normal distributions.
*   **`np.var`**: For empirical variance calculation across projected datasets.

### 📊 Matplotlib (Visualization)
Used to bring mathematical concepts to life:
*   **`plt.quiver`**: To visualize vectors and their relative angles (orthogonality).
*   **`plt.hist`**: To demonstrate the Central Limit Theorem through distribution shapes.
*   **`plt.scatter`**: To plot 2D point clouds representing multivariate Gaussian distributions.
*   **`plt.subplot`**: To compare "Before" (Standard Noise) and "After" (Covariance Transformation) states side-by-side.
*   **`plt.axhline` & `plt.axvline`**: To provide clear geometric references for the origin and axes.

## 📈 Visual Insights
The included Jupyter Notebook contains several visualizations:
- Orthogonality of vectors.
- Principal components as eigenvectors.
- The convergence of summed uniform noise to a bell curve.
- 2D Multivariate Gaussian point clouds.
