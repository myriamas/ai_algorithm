# Biscuit Optimization Project

## Overview
This project addresses a biscuit placement optimization problem: how to maximize the total value of biscuits placed on a dough roll while respecting defect constraints and reducing unused space.

We implemented and compared multiple optimization strategies, each with different strengths and trade-offs.

---

## Problem Setup
- The **dough roll** is modeled as a one-dimensional array of length 500.
- **Defects** are stored in a dictionary mapping each position to defect counts.
- **Biscuits** are defined by their length, value, and defect tolerance thresholds.

This representation enables efficient constraint checking during placement.

---

## Methods Implemented

### **1. Greedy Strategy**
Sorts biscuits from largest to smallest and places them sequentially.  
**Pros:** fast, simple.  
**Cons:** leaves gaps, often suboptimal.

### **2. Genetic Algorithm (GA)**
Uses tournament selection, crossover, mutation, and elitism to evolve better placements.  
**Pros:** robust, explores diverse solutions.  
**Cons:** parameter-sensitive.

### **3. Dynamic Programming (DP)**
Computes the optimal placement using recursion and memoization.  
**Pros:** guarantees the optimal result.  
**Cons:** computationally expensive.

### **4. Simulated Annealing (SA)**
Explores solutions probabilistically with a decreasing temperature schedule.  
**Pros:** escapes local optima.  
**Cons:** relies on tuning the cooling schedule.

---

## Key Insights
- **DP** serves as the optimal benchmark.  
- **GA** provides the best compromise between computation time and solution quality.  
- **SA** effectively avoids local minima.  
- **Greedy** offers a simple baseline for comparison.

This project illustrates how different optimization approaches behave under constrained placement requirements.

---
