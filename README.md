# Genetic Algorithm to solve 0/1 Knapsack Problem

This project uses a Genetic Algorithm (GA), a type of metaheuristic, to solve the 0/1 Knapsack problem, where the goal is to maximize the total value of items in a knapsack while respecting a weight limit.

## Problem Description

In the 0/1 Knapsack problem, you are given a set of items, each with a weight and a value. The objective is to select a subset of items such that the total weight is less than or equal to a given capacity and the total value is maximized.

- **Items**: Defined by their value and weight.
- **Knapsack capacity (MW)**: The maximum weight the knapsack can carry.

This project applies a Genetic Algorithm to find an optimal or near-optimal solution to this problem.

To learn more about the underlying concepts, check out the following resources:
- [Genetic Algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm)
- [0/1 Knapsack Problem](https://en.wikipedia.org/wiki/0/1_knapsack_problem)

## Genetic Algorithm Approach

1. **Chromosome Representation**: Each solution is represented as a chromosome (binary vector), where each gene corresponds to whether a specific item is selected (1) or not (0).
2. **Population**: A population of chromosomes is initialized randomly. Each chromosome undergoes genetic operations (selection, crossover, mutation) to evolve towards better solutions.
3. **Fitness Function**: The fitness of a chromosome is determined based on the total value of the selected items, penalized if the total weight exceeds the knapsack's capacity.
4. **Genetic Operations**: 
   - **Selection**: Individuals are selected based on their fitness, with better individuals having a higher chance of reproducing.
   - **Crossover**: Two chromosomes combine to form offspring with a mix of traits from both parents.
   - **Mutation**: Random mutation of genes to maintain diversity in the population and avoid premature convergence.

## Features

- **Chromosome Class**: Defines the structure of an individual solution, including the genes (binary representation), fitness calculation, and mutation.
- **Population Class**: Manages a population of chromosomes, including initialization, sorting by fitness, and displaying results.
- **Fitness Calculation**: Penalizes solutions that exceed the knapsack capacity and maximizes the total value of selected items.
- **Visualization**: Plots the evolution of the population's fitness over generations to observe the algorithm's convergence.


## Requirements

- Python 3.x
- `matplotlib` (for plotting and visualization)

## License

This project is licensed under the MIT License.



