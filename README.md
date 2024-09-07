# Aufgabe 2: Neville's Algorithm - Maple Implementation

This repository contains the solution to **Aufgabe 2** from the Maple seminar, focused on implementing Neville's algorithm for polynomial interpolation. The goal of this task is to compute the interpolation polynomial for a given set of data points.

## Problem Description

### Neville's Algorithm
Neville's method is a recursive algorithm used to find an interpolating polynomial that passes through a set of points \((x_i, y_i)\). The recursive formula is:

\[
p_{j,k}(x) = p_{j,k-1}(x) - \frac{(x_j - x)(p_{j,k-1}(x) - p_{j-1,k-1}(x))}{x_j - x_{j-k}}
\]

Where:
- \(p_{j,1}(x) = y_j\), for \( j = 1, \dots, n \)
- \( P(x) = p_{n,n}(x) \) is the final interpolating polynomial.

## Key Features
- **Polynomial Interpolation** using Neville's method.
- **Visualization** of the resulting interpolating polynomial.

## Example Dataset

This implementation has been tested with the following dataset:

| i  | 1  | 2  | 3  | 4  | 5  |
|----|----|----|----|----|----|
| \(x_i\) | -1 | 0  | 1  | 2  | 3  |
| \(y_i\) | 0  | -2 | 3  | 1  | 2  |

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/theprajwalm/maple.git
