# Markov2026

Coursework for Markov Processes. Each notebook holds the computational
parts of one homework problem — the analytic work is on paper, so the
notebooks generally pick up at the simulation or numerical part.

## Contents

| Notebook | Problem | What it does |
|---|---|---|
| `HW1_problem6.ipynb` | HW1 P6 | Monte Carlo estimate of `P(X²+Y²<Z, Z²>XY)` for independent Uniform[0,1] variables, converging to the analytic value `23π/192` as sample size grows from 10 to 10⁴ |
| `HW2_problem5.ipynb` | HW2 P5 | Three sampling assignments: accept–reject sampling of `f(x)=xe^{-x}`, a two-component exponential mixture, and inverse-transform sampling with a reinforcement scheme |
| `HW3_problem1.ipynb` | HW3 P1 | Long-run behavior of a 3-state chain via `P⁵⁰` |
| `HW3_problem2.ipynb` | HW3 P2 | A 6-state chain with transient and absorbing structure, examined through `P²¹` |
| `HW3_problem4.ipynb` | HW3 P4 | Lamb-and-lion survival problem: random walks with one and two lions, fitting the survival exponent β and comparing against the continuum prediction `erf(d₀/2√t)` |

## Running

The notebooks use NumPy, Matplotlib, and SciPy:

```
pip install numpy matplotlib scipy jupyter
jupyter notebook
```

Simulations seed via `np.random.default_rng()`, so results vary slightly
between runs except where an explicit seed is passed.

## Author

Filippa Mudsam
