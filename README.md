# Linear Regression Solver

Starter repository for the **Numerical Computing** capstone on [DutchEngineer](https://dutchengineer.org).

## What you will build

A linear regression solver implemented from scratch in NumPy — no machine learning libraries, no black boxes. Two approaches, both validated against a reference implementation. The constraint is the point: when your coefficients match to floating-point precision, you know you understand the matrix math, not just the API.

## Requirements

1. **Closed-form solver** — find weights in a single pass with no iteration. Handle the bias term without a separate variable. Handle ill-conditioned inputs without crashing, and document when that fallback activates.
2. **Iterative solver** — find weights by repeatedly updating them in the direction that reduces error. No external optimisation library. Track loss across iterations.
3. **Validation against reference** — both solvers must produce coefficients and predictions that match scikit-learn's LinearRegression on the same dataset, within a tolerance you can justify.
4. **Performance comparison** — measure wall-clock time for both methods on a large dataset. Write up which is faster and why in a `RESULTS.md` file — the explanation matters as much as the numbers.
5. **Test suite** — tests verify: both solvers match the reference, the ill-conditioned fallback does not raise, and loss decreases across iterations. All tests pass from a clean install.

## Getting started

1. **Fork this repository** — click **Fork** at the top of [this page](https://github.com/dutchengineer-org/linear-regression-solver-starter) to create your own copy.
2. Clone your fork:
   ```
   git clone https://github.com/<your-username>/linear-regression-solver-starter
   cd linear-regression-solver-starter
   ```
3. Install dependencies: `uv sync`
4. Build and run: `uv run pytest && uv run python benchmark.py`

## Submitting

When your work is ready, paste your repository URL into the submission form on your [capstone page](https://dutchengineer.org/foundations/numerical-computing/capstone-linear-regression-solver/).
