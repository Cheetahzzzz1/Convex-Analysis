# Convex-Analysis

# Overview

This assignment provides a computational verification of the convexity of the set of positive semidefinite (PSD) matrices. The convexity property states that if two matrices are PSD, their convex combination remians PSD.

# Problem Statement

![Screenshot 2025-03-03 164037](https://github.com/user-attachments/assets/88bd864f-5a45-4535-8f61-90f871d7c3ca)

The problem statement states that the matrix 

             C = λA + (1-λ)B

must also be a PSD.

# Methodology

(a) <ins> Definition of Positive Semidefiniteness </ins>

A symmetric matrix M is positive semidefinite (PSD) if all it's eigenvalues are nonnegative:

$M \succeq 0 \iff \forall x \in \mathbb{R}^n, x^T M x \geq 0.$

(b) <ins> Checking Convexity </ins>

To verify convexity, we:

1. Generate two random PSD matrices A and B.

2. Compute their convex combination C.

3. Check if C is PSD by verifying that all its eigenvalues are nonnegative.

(c) <ins> Computational Verification </ins>

1. We use NumPy to generate symmetric PSD matrices by computing A = MM^T for a random matrix M.

2. The eigenvalues of C are computed using numpy.linalg.eigvalsh to verify its positive semidefiniteness.

# Implementation

The computational approach involves:

1. Generating random PSD matrices.

2. Computing their convex combination.

3. Checking whether the resulting matrix is PSD.

# Results

1. The convex combination C was found to be positive semidefinite, confirming that S^n is convex.

2. The eigenvalue analysis demonstrated that all eigenvalues of C were nonnegative, satisfying the definition of positive semidefiniteness.

# Dependencies

1. Python 3

2. NumPy

3. Pandas

# Conclusion

The problem was successfully solved, confirming that the set of positive semidefinitematrices is convex both mathematically and computationally.
