# APD Conjecture Verification Suite

## Overview
This program calculates the **Alternating Power Difference (APD)** for various types of matrices ($n=2$ to $n=7$) and identifies the degree $m$ at which the APD first becomes non-zero ($m_1$). 

The goal is to empirically support the following conjecture for any square matrix $A$ where $m_1(A) < \infty$:

$$n-1 \le m_1(A) \le \frac{n(n-1)}{2}$$

## Key Features
- **Exact Arithmetic**: Uses Python's arbitrary-precision integers and the `fractions` module to eliminate floating-point errors.
- **Reproducibility**: Uses a fixed seed (`np.random.seed(42)`) to ensure identical results across different environments.
- **Diverse Matrix Types**: Tests integer, sparse, singular, and rational matrices.
- **Complete Search**: Exhaustively computes all $n!$ permutations for $n \le 7$.

## Requirements
- Python 3.x
- NumPy

## How to Run
```bash
python apd_verification.py