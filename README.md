# Fifteen-Puzzle-Solver
First assignment of the course Artificial Intelligence (2nd year, 2nd semester)

## A little context
### Problem Description
The Fifteen Puzzle is represented by a 4x4 matrix containing 15 numbered cells and one empty cell. Variations of this game may involve part of an image in each cell. The problem consists of starting from a shuffled initial configuration of the cells and reaching a final configuration with a determined order of digits (in the case of the number matrix) or images (in the case of the matrix where cells represent parts of an image). The possible movements/operators to go from one configuration to another are: 1) move the empty cell up, 2) move the empty cell down, 3) move the empty cell right, and 4) move the empty cell left.

Note: For some sets of initial and final configurations, this problem, as well as its reduced version - the eight puzzle, has no solution. This subject was investigated and implemented in the program through a code that verifies if, for a given initial configuration of the Fifteen Puzzle, there is a path that leads to the final solution, without performing any search. 

### Implementation
The following search strategies were implemented:

* Iterative Depth-First Search
* A*
* Greedy Best-First Search with heuristics
* Depth-First Search
* Breadth-First Search

### Heuristics
For the implementation of the A* and Greedy Best-First strategies, two heuristics were used: 
* sum of the number of pieces out of place
*  Manhattan distance (sum of the distances from each piece to its place in the final configuration).

Given the initial and final configurations (which are input arguments to the program), the operators used in the path leading to the solution, number of steps, execution time, and amount of memory used (counted as the maximum number of nodes stored simultaneously in memory during execution) are printed.

### Stats
For each strategy, were analyzed the following statistics:

* Time taken to reach a solution,
* Amount of space used (number of generated and stored nodes),
* Completeness (can the algorithm find a solution?) and
* Optimality (What is the depth of the solution found? Does the found solution correspond to the smallest number of steps to reach the final configuration or with the lowest cost using little time and memory?)
* Use graphs or tables to compare the various strategies.

At the end all the strategies were compared.



