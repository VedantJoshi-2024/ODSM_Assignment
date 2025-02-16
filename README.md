# Optimization and Data Science Methods Assignment
## Table of Contents <br>

1. [Introduction](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#introduction)

2. [Part A: Warm-up](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#part-a-warm-up)

- [A1. Gradient Descent Recap](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#a1-gradient-descent-recap)
- [A2. Newton's Method](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#a2-newtons-method)
- [A3. Hessian & Local Optimality](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#a3-hessian--local-optimality)

3. [Part B: Applied Coding Tasks](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#part-b-applied-coding-tasks)

- [B1. Minimizing a Real Function](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#b1-minimizing-a-real-function)
- [B2. Small Data Problem](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#b2-small-data-problem)

4. [Part C: Conceptual Intuition on Quasi-Newton vs. Exact Newton](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#part-c-conceptual-intuition-on-quasi-newton-vs-exact-newton)

5. [Conclusion](https://github.com/VedantJoshi-2024/ODSM_Assignment/tree/main?tab=readme-ov-file#conclusion)

### Introduction
This repository contains the solutions and explanations for an assignment focused on optimization techniques and data science methods. The assignment is divided into three main parts: theoretical warm-up exercises, applied coding tasks, and conceptual questions about Newton and quasi-Newton methods.

### Part A: Warm-up
#### A1. Gradient Descent Recap
In this section, we explore the fundamentals of gradient descent, explaining why the update rule:

```{text}
w_{k+1} = w_{k} - α∇f(w_{k})
```
leads us closer to a (local) minimum. We discuss:<br>
- The concept of steepest descent
- The importance of choosing a suitable step size α
- An example using the function f(ω) = ω₁² + ω₂²
- Comparison between fixed step size and Armijo line search methods

#### A2. Newton's Method
This section focuses on Newton's method applied to the function:

```{text}
f(x) = x⁴ - 4x² + 5
```
We cover:<br>
- Derivation of f'(x) and f''(x)
- The Newton update formula in 1D
- Manual computation of x₁ and x₂ starting from x₀ = 2
- Analysis of convergence towards a local minimum

#### A3. Hessian & Local Optimality
Here, we discuss the Hessian matrix and its role in determining local optimality. Key points include:
- Interpretation of eigenvalues for identifying local maxima, minima, or saddle points
- Explanation of critical points when the Hessian has both positive and negative eigenvalues

### Part B: Applied Coding Tasks
#### B1. Minimizing a Real Function

In this coding task, we implement and compare gradient descent and Newton's method for minimizing a 2D function:

```{python}
f(x0, x1) = (1-x0)² + 100(x1 - x0²)²
```
The implementation includes:
- Function definitions for f(x,y), gradient, and Hessian
- Gradient descent and Newton's method algorithms
- Visualization of iteration paths using contour plots
- Comparison of iteration counts, final accuracies, and gradient norms

#### B2. Small Data Problem

This section explores the use of different optimization algorithms on small datasets:

1. Logistic Regression on the Iris dataset
2. Linear Regression on the Diabetes dataset

We compare various solvers including:
- LBFGS
- Newton-CG
- SAGA

The analysis covers:
- Accuracy and iteration counts for classification tasks
- Mean Squared Error (MSE) for regression tasks
- Discussion on the performance of different solvers

### Part C: Conceptual Intuition on Quasi-Newton vs. Exact Newton

This section provides insights into the choice between quasi-Newton and exact Newton methods:

- Advantages of quasi-Newton methods for large-scale problems
- Considerations for datasets with high-dimensional features (e.g., 50,000 features)
- Practical observations from using quasi-Newton methods in Part B

### Conclusion
The assignment demonstrates a comprehensive understanding of optimization techniques in data science, from theoretical foundations to practical implementations. It highlights the trade-offs between different methods and their applicability to various problem sizes and types.

For more details on each section, please refer to the corresponding parts in the assignment document. The code implementations and detailed explanations can be found in the respective files within this repository.
