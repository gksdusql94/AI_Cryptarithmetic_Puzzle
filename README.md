# Cryptarithmetic Puzzle Solver

## Overview
The **Cryptarithmetic Puzzle Solver** is a Python-based tool that solves cryptarithmetic puzzles where letters represent digits, and the goal is to replace each letter with a unique digit such that a given arithmetic operation (usually addition) holds true. The solution involves mapping letters to digits while maintaining the arithmetic validity of the equation.

## Algorithm
The solver uses **brute-force search** by:
1. Generating all possible permutations of digits (0-9) that can replace the unique letters in the puzzle.
2. Applying the generated permutations to check if the resulting arithmetic operation holds true.
3. Printing the valid mapping of letters to digits if a solution exists.

The approach ensures that no two letters share the same digit, and the leading digit of any number is not zero.

## Features
- Solves any cryptarithmetic puzzle with up to 10 unique letters.
- Returns all possible solutions where the puzzle constraints are satisfied.
- Handles puzzles with word inputs for two operands and one result.

## Installation
Ensure you have Python 3 installed on your system. No external libraries are required for this project.

## Usage
1. Clone the repository or download the script.
2. Run the script:
   ```bash
   python cryptarithmetic_puzzle_solver.py
## Example

    SEND
+   MORE
-------
  MONEY

## Solutions:
S = 9
E = 5
N = 6
D = 7
M = 1
O = 0
R = 8
Y = 2

## How It Works
The puzzle words are treated as numbers with unknown digits represented by letters.
A set of all letters is created from the input words.
The solver tries every possible permutation of the digits 0-9 for the letters.
The program checks if any permutation satisfies the condition word1 + word2 = result.

## Limitations
The solver only supports puzzles with a maximum of 10 unique letters due to the digit constraint (0-9).
The solution might take time depending on the number of unique letters, as the number of possible permutations grows exponentially.
