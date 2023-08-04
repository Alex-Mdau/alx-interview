#N Queens Puzzle Solver

The N queens puzzle is a classic problem of placing N non-attacking queens on an N×N chessboard. This program solves the N queens problem using backtracking.
Usage

To use the program, run the following command in the terminal:

mathematica

nqueens N

where N is an integer greater than or equal to 4, representing the size of the chessboard and the number of queens to be placed.
Examples

If the user calls the program with the wrong number of arguments, the program will display the usage information and exit with status 1:

makefile

Usage: nqueens N

If N is not an integer, the program will display the following message and exit with status 1:

css

N must be a number

If N is smaller than 4, the program will display the following message and exit with status 1:

mathematica

N must be at least 4

The program will print every possible solution to the N queens problem, one solution per line, in the following format:

lua

[[row1, col1], [row2, col2], ..., [rowN, colN]]

You don't have to print the solutions in a specific order.
Examples

css

$ ./nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]

$ ./nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]

Note

This program only imports the sys module for handling command line arguments.
