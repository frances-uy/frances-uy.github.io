---
layout: project
type: project
image: img/An-example-Sudoku-puzzle.png
title: "Recursive Sudoku Solver"
date: 2023
published: true
labels:
  - Java
  - Recursion
summary: "Sudoku Solver using a Backtracking algorithm."
---

## What is Sudoku?
Sudoku, a popular combinatorial-number puzzle involving logic and reasoning, can be tedious and frustrating if played by a human. Especially while starting it out. The goal of Sudoku is to fill a 9 × 9 grid with digits so that each column, each row, and each of the nine 3 × 3 subgrids that compose the grid contain all of the digits from 1 to 9.

## How Does It Work?
This Sudoku Solver uses backtracking, a brute-force algorithm which tries different numbers. If it fails, then it backtracks and tries another number. If none of the numbers work, then no solution will be found. It's simple and effective. Test cases were provided by the instructor, and I had the responsibility of implementing a function that actually filled in the numbers.

This individual assignment from ICS 211 reinforced my knowledge of recursion, a significant topic in Computer Science. This was done in Java and used other data structures such as arrays.

_Here is a snippet of my code, one of the functions I implemented:_
```
 /*
   * find an assignment of values to sudoku cells that makes the sudoku valid
   * @param the sudoku to be filled
   * @return whether a solution was found 
   *    if a solution was found, the sudoku is filled in with the solution
   *    if no solution was found, restores the sudoku to its original value
   */
  public static boolean fillSudoku (int [][] sudoku) {
      //keeps track of whether or not the puzzle has been fully filled
      boolean allFilled = true;
      //do not forget to update these values later
      int row = -1;
      int col = -1;

      for (int i = 0; i < sudoku.length; i++) {
          for (int j = 0; j < sudoku.length; j++) {
              int cell = sudoku[i][j];
              if (cell == 0) {
                  row = i;
                  col = j;
                  allFilled = false;
                  break;
              }
          }
          if (!allFilled) {
              break;
          }
      }

      if (allFilled) {
    	// solution found
          return true; 
      }
      for (int num = 1; num <= 9; num++) {
          sudoku[row][col] = num;
          if (checkSudoku(sudoku, allFilled)) {
              if (fillSudoku(sudoku)) {
            	// solution found
                  return true; 
              }
          }
          // restoring the assignment
          // try the next number, still in for loop
          sudoku[row][col] = 0; 
      }
      //no solution found
      return false; 
  }
}

```
