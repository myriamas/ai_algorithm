Biscuit Optimization Project
Overview

This project tackles a biscuit placement optimization problem: how to maximize the total value of biscuits placed on a dough roll while respecting defect constraints and minimizing unused space.
We explored and compared several optimization strategies, each with different trade-offs in efficiency, accuracy, and computational cost.

Problem Setup

The dough roll is modeled as a 1D array of length 500.

Defects are stored as a dictionary mapping each position to defect counts.

Biscuits are represented by their length, value, and acceptable defect thresholds.

This structure allows efficient validation of placements and constraint checking.

Methods Implemented
1. Greedy Strategy

Places biscuits from the largest to the smallest.

Pros: very fast, simple, low computational cost

Cons: leaves gaps, not optimal

2. Genetic Algorithm (GA)

Uses tournament selection, crossover, mutation, and elitism to evolve better placements.

Pros: robust, explores many configurations

Cons: sensitive to parameter tuning

3. Dynamic Programming (DP)

Computes the optimal solution by exploring all valid placements with memoization.

Pros: guarantees the best possible result

Cons: computationally expensive

4. Simulated Annealing (SA)

Probabilistically explores the search space with a cooling schedule.

Pros: escapes local optima

Cons: performance depends heavily on temperature settings

Key Insights

DP provides the optimal benchmark solution.

GA offers the best balance between quality and computation time.

SA is useful for escaping local minima.

Greedy serves as a quick and simple baseline.

This project highlights how different optimization paradigms perform when handling constrained placement problems.
