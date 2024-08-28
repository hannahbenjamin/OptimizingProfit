# Optimizing Profit

## Overview

This project aims to optimize the production plan for WARP Shoe Company to maximize profit, given a doubled demand for February 2006. Using integer programming and linear programming techniques, we developed a model to determine the optimal number of shoes to produce while adhering to constraints related to raw materials, warehouse capacity, machine time, and demand.

## Project Details

**Date:** December 1, 2023  
**Authors:** Hannah Benjamin (1008991307), Anika Mule (1008850325)  
**Course:** MIE 262

## Problem Statement

The goal was to formulate a production plan that maximizes profit while considering constraints such as raw materials budget ($10,000,000), warehouse capacity, machine operation time (12 hours/day for 28 days), and available raw materials.

## Methodology

### Assumptions

- All shoes require specific components.
- Demand for February is estimated based on historical data.
- Transportation and machine setup costs are excluded.
- Machines operate a maximum of 20,160 minutes/month.
- Raw materials budget is fixed at $10,000,000.

### Integer Programming Formulation

- **Decision Variable:** Number of pairs of each shoe type produced.
- **Parameters:** Prices, demands, costs of raw materials, operation times, etc.
- **Objective Function:** Maximize profit by balancing production and constraints.
- **Constraints:** Budget limits, warehouse capacity, machine time, material availability, non-negativity.

### Solution Approach

- Utilized AMPL and Gurobi solver.
- Relaxed integer program to linear program due to high computation time.
- Resulted in a maximum profit of $13,458,506.80.

## Results

- **Optimal Profit:** $13,458,506.80
- **Files Used:**
  - `warp.mod`: Model file with sets, parameters, decision variables, and constraints.
  - `warp.dat`: Data file for parameters.
  - `warp.run`: Run file to execute the model.
  - `warp.out`: Output file with results.
- **Key Findings:**
  - Constraints related to available raw materials were binding.
  - Warehouse capacity was not a limiting factor.
  - Reducing machine hours had minimal impact on profit, indicating a non-binding constraint.

## Additional Considerations

- **Demand Estimation:** Calculated using historical data from 1997-2003.
- **Variable and Constraint Count:** Detailed in the report.
- **Sensitivity Analysis:** Examined effects of additional warehouse space and increased raw materials budget.

## Conclusion

The project successfully optimized the production plan for WARP Shoe Company, achieving the maximum possible profit given the constraints. The results and methodology are detailed in the provided files and documentation.

For further details on the modeling and results, refer to the full report and appendices.
