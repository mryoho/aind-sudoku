# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: Constraint Propagation allows us to filter the search space to make a
complex search problem simpler to solve. One of the constraints that applies
to solving a Sudoku is the Naked Twins technique. The naked twins technique
posits that the existence of two boxes with the same two-digit possibilities
implies that each one of those digits must end up in one of those two boxes
and those two numbers can thus show up nowhere else in a unit. Therefore, those
two numbers can be eliminated from all of the other boxes in the unit. This
technique has been implemented in code.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: The typical Sudoku puzzle only requires that the numbers 1-9 only show up
once in each row, column, and square of 9 boxes. The diagonal sudoku problem on
the other hand also requires that the two 9 box diagonals also only include the
digits 1-9 a single time. Fortuitously, this additional constraint does not
rule out the constraint propagation techniques that we have already applied, but
rather only requires the redefinition of the boxes that are considered peers.
Once that modification has been made to include those boxes, the Naked Twins,
Elimination, and Only Choice techniques all still apply for finding a solution
to the diagnol sudoku problem. The peer modification has been implemented in
code.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
