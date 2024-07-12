## GraphPlan Planner

This project implements the GraphPlan planning algorithm and additional heuristic search methods for solving AI planning problems.

## Overview

GraphPlan is an algorithm used in automated planning in artificial intelligence. It constructs a planning graph, a layered structure that alternates between levels of actions and propositions, and uses it to efficiently find a sequence of actions that lead from the initial state to the goal state.

## Key Components

### `planning_problem.py`
Encapsulates the planning problem, including:
- Parsing domain and problem files.
- Managing the initial and goal states.
- Defining actions and propositions.
- Implementing heuristic functions for search guidance.

### `graph_plan.py`
Implements the GraphPlan algorithm, including:
- Constructing and expanding the planning graph.
- Extracting a valid plan from the graph using backward search.
- Handling no-ops and independent actions for efficient planning.

### Other Supporting Files
- `proposition.py` and `proposition_layer.py`: Define propositions and their layers within the planning graph.
- `action.py` and `action_layer.py`: Define actions and their layers within the planning graph.

## Usage

To run the GraphPlan algorithm or heuristic search on a planning problem, use the following command:
```python
python planning_problem.py domain_file problem_file heuristic_name
```


## Heuristics

The following heuristics are available for guiding the search process:
- `max`: Uses the maximum level heuristic.
- `sum`: Uses the level sum heuristic.
- `zero`: Uses a null heuristic (equivalent to no heuristic).

## Example Domain and Problem Files

Example domain and problem files (e.g., `hanoi_2_3_domain.txt`, `hanoi_2_3_problem.txt`) are provided to demonstrate the functionality of the planner.

