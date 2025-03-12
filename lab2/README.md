#### Andrea Zenotto - s327473

---

# Lab2: Traveling Salesman Problem (TSP) Solution

## Overview
This project implements solutions for the Traveling Salesman Problem (TSP) using two different approaches: a fast but approximate algorithm and a slower, yet more accurate genetic algorithm. The goal is to demonstrate the trade-offs between speed and accuracy in solving TSP instances.

## Algorithms Used

### 1. Nearest Neighbor Algorithm
- **Description**: This is a heuristic approach that constructs a solution by repeatedly visiting the nearest unvisited city until all cities have been visited. This method is fast and provides a good initial solution, although it may not yield the optimal path.
  
### 2. Genetic Algorithm
- **Description**: A more accurate method that uses principles of natural selection and genetics to evolve a population of solutions over multiple generations. It employs crossover and mutation operators to explore the solution space.
- **Crossover Techniques**: 
  - Order 1 Crossover (OX1)
  - Inversion Crossover
- **Mutation Techniques**:
  - Single Mutation (swapping two cities)
  - Inversion Mutation (reversing the order of a segment of the path)

### Implementation Details
- **Population Size**: Set to 100 for the genetic algorithm, balancing exploration and computation time.
- **Offspring Size**: Set to 50, ensuring diversity in the new generation.
- **Generations**: Varies depending on the country (instance), allowing flexibility based on the complexity of the problem.
  
## Results
The following table summarizes the results obtained for each country using both the Nearest Neighbor (NN) algorithm and the Genetic Algorithm:

| Country | Nearest Neighbor Distance | Genetic Algorithm Distance |
|---------|---------------------------|----------------------------|
| Vanuatu | 1,475.73 km               | 1,475.53 km                |
| Italy   | 4,436.03 km               | 4,201.69 km                |
| Russia  | 42,334.16 km              | 34,472.24 km               |
| US      | 48,050.03 km              | 41,632.50 km               |
| China   | 63,962.92 km              | 58,706.00 km               |

