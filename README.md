# COSC 111 Exam 4

In the exam, you will be asked to determine if a matrix is a Latin square or not.

http://mathworld.wolfram.com/LatinSquare.html (Links to an external site.)

## Part 1

Complete the methods findInRow and findInColumn.

   - findInRow: Given row i and value val, it returns the column where val was found. Otherwise, returns -1. For example, if we have a row i with values [2 1 3] and val is 2, it should return 0. If val is 3, it should return 2. If val is 4 it should return -1.
   - findInColumn: Same as findInRow but have to find in a column.

There are two unit tests (FindInRowsTest and FindInColumnsTest) that should pass.

## Part 2

Write the methods isRowLatin, isColumnLatin and isLatin in the class LatinSquare.

   - isRowLatin: if the row has numbers 1, ..., n (n is the number of columns) somewhere in the row, then return true. If a number is missing and not in the row, return -1. For example, the row [2 1 3] is Latin but [1 2 1] is not Latin.
   - isColumnLatin: Same as isRowLatin but for a column
    isLatin: all the rows and columns are Latin.

There are 4 unit tests (LatinTest*) that should pass when you have implemented the functions correctly.

## Part 3 (Optional - Extra Credit)

When you run LatinSquaresApp, it will print out the matrix and say if it Latin or not.

Modify it so that it also prints out if each row and column is Latin or not.

For example. for *Test4.txt* should output,

~~~~
[1 2 3 ]
[1 3 2 ]
[2 1 3 ]
rows: [true true true ]
cols: [false true false]
false
~~~~
