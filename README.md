# Probabilistic Artificial Intelligence

Course projects for *Probabilistic Artificial Intelligence*, ETH Zurich, autumn 2022. Group projects in
Python.

| Task | Problem | Approach |
| --- | --- | --- |
| [1](task1-gaussian-process-regression) | Predict pollution concentration with Gaussian process regression, where underpredicting costs much more than overpredicting | Rational quadratic + white noise kernel, fitted on a subsample of the data to keep it tractable; predicts mean + 0.13 × std to account for the uneven cost |
| [3](task3-bayesian-optimization) | Find the maximum of an expensive black-box function while keeping a speed constraint satisfied | Bayesian optimization with Gaussian processes for the objective and the constraint (Matérn + white + constant kernels) and an expected-improvement acquisition function |
| [4](task4-reinforcement-learning) | Teach a lunar lander to land | Actor-critic policy gradient with rewards-to-go and TD residuals. [`policy.mp4`](task4-reinforcement-learning/policy.mp4) is a recorded run of a trained policy |

Each folder has `solution.py` and the course's `requirements.txt`. The datasets and the course's
grading tools are not included.
