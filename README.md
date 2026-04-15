# CSP-Sudoku-Solver-Report

Overview

This project implements a Sudoku solver using a Constraint Satisfaction Problem (CSP) approach. The solver combines Backtracking Search, AC-3 Constraint Propagation, Forward Checking, and the MRV heuristic to efficiently solve Sudoku puzzles of varying difficulty.

Features
Solves standard 9×9 Sudoku puzzles
Uses CSP techniques for efficient solving
Implements:
Backtracking Search
AC-3 Algorithm
Forward Checking
MRV (Minimum Remaining Values)
Tracks performance:
Number of backtrack calls
Number of backtrack failures
Displays solution in a formatted 3×3 grid
File Structure
project/
│
├── sudoku_csp_solver.py   # Main solver code
├── easy.txt               # Easy Sudoku puzzle
├── medium.txt             # Medium Sudoku puzzle
├── hard.txt               # Hard Sudoku puzzle
├── veryhard.txt           # Very hard Sudoku puzzle
└── README.md              # Project documentation
Input Format

Each Sudoku puzzle file must follow this format:

Exactly 9 lines
Each line contains 9 digits (0–9)
0 represents an empty cell
Example:
004030050
609400000
005100489
000060930
300807002
026040000
453009600
000004705
090050200
How to Run
Place all .txt files in the same directory as the Python file.
Run the program:
python sudoku_csp_solver.py
The solver will:
Read each puzzle
Solve it
Print the solution
Display backtracking statistics
Output Example
===== easy.txt =====

Solved Sudoku:
+-------+-------+-------+
| 7 8 4 | 9 3 2 | 1 5 6 |
| 6 1 9 | 4 8 5 | 3 2 7 |
| 2 3 5 | 1 7 6 | 4 8 9 |
+-------+-------+-------+
...

Backtrack Calls: 82
Backtrack Failures: 0
Results Summary
Easy, Medium, Hard puzzles were solved with no failures
Very Hard puzzle required backtracking with some failures
AC-3 significantly reduced the search space
MRV improved efficiency by selecting optimal variables
Technologies Used
Python 3
Standard libraries:
collections
copy
Conclusion

This project demonstrates the effectiveness of CSP techniques in solving Sudoku problems. The combination of AC-3, backtracking, forward checking, and heuristics results in an efficient and scalable solver.

Author

MUHAMMAD SHAHEER
