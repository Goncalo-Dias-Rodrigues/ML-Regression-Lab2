# ML-Regression-Lab2

# Simple Linear Regression — ML Lab 2

Jupyter Notebook implementation of simple linear regression, developed as Lab 2 for the Machine Learning course. The project covers closed-form (normal equation / OLS) and gradient descent approaches to fitting a regression line, along with residual analysis and cost function visualization.

## Overview

Using a dataset relating **years of experience** to **salary**, this project:

- Computes the line of best fit (θ₀*, θ₁*) two ways:
  - `scipy.stats.linregress()`
  - A NumPy implementation of the closed-form OLS solution
- Verifies both methods produce equivalent results
- Visualizes the dataset with the fitted regression line
- Predicts `y` for a given `x` and computes/plots the residual
- Interprets the slope and intercept in the context of the data
- Uses the model to extrapolate a prediction (20 years of experience)
- Expresses and computes the cost function `J(θ₀, θ₁)` in vector notation
- Proves analytically that:
  - The point (x̄, ȳ) lies on the regression line
  - The sum of residuals is zero
- Plots residuals vs. the independent variable, with their mean and variance
- Derives the partial derivatives of the cost function
- Implements **gradient descent** in vector notation and compares its results (θ values, cost, iterations, learning rate) to the closed-form solution
- Plots the cost function `J` as a function of gradient descent iterations

## Repository Structure in "src" directory

```
.
├── regression-intro.ipynb     # Introductory notebook (provided)
├── demodataset.csv            # Dataset used in the introductory notebook
├── Lab2-regression.ipynb      # Main assignment notebook with answers
└── README.md
```

## Requirements

- Python 3.x
- Jupyter Notebook
- NumPy
- SciPy
- Matplotlib
- Pandas (if used for data loading)

Install dependencies with:

```bash
pip install numpy scipy matplotlib pandas jupyter
```

## Usage

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```
2. Launch Jupyter Notebook in the "src" directory:
   ```bash
   jupyter notebook
   ```
3. Open `Lab2-regression.ipynb` and run all cells in order.

## Author

had, jvo — Machine Learning course, Lab 2: Simple Linear Regression.

## References

- [Jupyter Notebook](https://jupyter.org/)
- [Math Is Fun — List of Derivative Rules](https://www.mathsisfun.com/calculus/derivatives-rules.html)
