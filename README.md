# Sudoku-GUI-Solver

file:///Users/ibrahimshehu/Downloads/sudoku.gif

This is a playable sudoku game that utilizes  the backtracking algorithm to solve the puzzle. It includes a graphical GUI as well as a text based version.

Every time the program is executed, a random, solvable board is created and the user can attempt to solve it by clicking on the cells. This board is created by using the Sengoku api to generate the values for the board. In the event that the user cannot connect to the api via the internet, a hardcoded board will be used. Entering a number into a cell will be entered as a tentative value. Once the the user is sure that the inputted number is the correct entry, pressing the enter key will input the number onto the board. 

# What is a Backtracking Alogorithm
Backtracking is a general algorithm for finding all (or some) solutions to some computational problems through a brute force approach, that incrementally builds candidates to the solutions, and abandons each partial candidate (“backtracks”) as soon as it determines that the candidate cannot possibly be completed to a valid solution

* Find the first empty space if it exist
* Attempt to place the digits 1-9 in that space
* Check if that digit is valid in the current spot based on the current board
* attempt the board with backtrack
* If the digit is valid, recursively attempt to fill the board using steps 1-3.
* If it is not valid, reset the square you just filled and go back to the previous step.
* Once the board is full by the definition of this algorithm we have found a solution.

Run GUI.py to play sudoku.

## Instructions:
- Zip Download the Repository and Extract it's contents.
-Install pygame
-python3 -m pip install pygame
- Now run the GUI.py file directly in your Terminal using
```
python GUI.py
```
**OR**
```
python3 GUI.py
```



# Instructions
Click a box and hit the number on your keybaord to input in a number. To confirm that value press the ENTER key on that box. To delete an input click DEL. Finally to solve the board press SPACE and watch the algorithm run.

## Input:

| Keys              | Actions                                                         |
|-------------------|-----------------------------------------------------------------|
| `Left Click`      | Selects the Box to enter a value into that cell.                |
| `Enter`           | Confirms the Value written on the board.     |
| `Backspace/Delete`| Deletes the value in that cell.                                 |
| `Space`           | Solves the Board using the Algorithm.                           |



# Sudoku
