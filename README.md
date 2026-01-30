# Mean-Variance-Standard-Deviation-Calculator

A Python utility that calculates statistical measures (mean, variance, standard deviation, max, min, and sum) for a 3x3 matrix using NumPy.

## Features

- **Mean**: Calculates the mean across columns, rows, and the entire matrix
- **Variance**: Computes variance across columns, rows, and the entire matrix
- **Standard Deviation**: Calculates standard deviation across columns, rows, and the entire matrix
- **Max**: Finds maximum values across columns, rows, and the entire matrix
- **Min**: Finds minimum values across columns, rows, and the entire matrix
- **Sum**: Calculates sums across columns, rows, and the entire matrix

## Requirements

- Python 3.x
- NumPy

## Installation

```bash
pip install numpy
```

## Usage

```python
from mean_var_std import calculate

# Input a list of 9 numbers
result = calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])

print(result)
```

The function takes a list of exactly 9 numbers and returns a dictionary with calculated statistics.

## Input Validation

- The input list must contain exactly 9 numbers
- Raises `ValueError` if the list doesn't contain exactly 9 numbers

## Output Format

Returns a dictionary with keys: `mean`, `variance`, `standard deviation`, `max`, `min`, `sum`

Each key contains a list with three elements:

- Index 0: Statistics calculated along columns (axis=0)
- Index 1: Statistics calculated along rows (axis=1)
- Index 2: Statistics calculated for the entire matrix
