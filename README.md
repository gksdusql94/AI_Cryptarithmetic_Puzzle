# 🔢 Cryptarithmetic Puzzle Solver

## 📝 Overview
The **Cryptarithmetic Puzzle Solver** is a Python-based tool designed to solve cryptarithmetic puzzles where letters represent digits. The objective is to replace each letter with a unique digit such that a given arithmetic equation (usually addition) holds true. The solver brute-forces through possible combinations of digits to find all valid solutions.

## 🧠 Algorithm
The solver uses a **brute-force search** approach:
1. Generates all possible permutations of digits (0-9) that can replace the unique letters in the puzzle.
2. Applies these permutations to check if the resulting arithmetic operation holds true.
3. Prints the valid mappings of letters to digits when a solution is found.

### 🔑 Key constraints
- Each letter is mapped to a unique digit.
- The first letter of any operand or result cannot be mapped to zero.

## 🌟 Features
- Solves any cryptarithmetic puzzle with up to 10 unique letters.
- Returns all possible solutions where the puzzle constraints are satisfied.
- Handles puzzles with two word-based operands and one word-based result.

## 💻 Installation
Ensure that you have Python 3 installed on your system. This project does not require any external libraries.

## 🚀 Usage
1. Clone the repository or download the script.
2. Run the script using the following command:
   ```bash
   python cryptarithmetic_puzzle_solver.py
3. When prompted, enter the two words representing the operands and the result word.

## 🔍 Example Puzzle

    SEND+   MORE = MONEY

## 📝 Solutions:
S = 9
E = 5
N = 6
D = 7
M = 1
O = 0
R = 8
Y = 2

![image](https://github.com/user-attachments/assets/bafc9601-b85b-4fee-92cf-2242e4d9333d)

## ⚙️How It Works
1. Input Parsing: The puzzle words are treated as numbers, with unknown digits represented by letters.
2. Letter Set Creation: A set of all unique letters is created from the input operands and result word.
3. Permutation Generation: The solver generates all possible digit permutations for the letters.
4. Validation: The program checks if any of the generated permutations satisfy the condition word1 + word2 = result.
   
## ⚠️Limitations
The solver only supports puzzles with a maximum of 10 unique letters due to the digit constraint (0-9).
The solution might take time depending on the number of unique letters, as the number of possible permutations grows exponentially.


### Improvements made:
1. **Clarity in headings**: Section headings are made more descriptive for easier navigation.
2. **Expanded explanation in "How It Works"**: Added clearer explanations of each step of the solver’s operation.
3. **Enhanced formatting**: Improved formatting for better readability.
4. **Incorporated your sample output**: Included the example output and image for better context.

