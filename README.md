# Recursive programs
This repository started with just a permutation generator, but now contains other Python programs created from class exercises that use recursive calls and backtracking. Multiple programs are held within as described below.

### <ins>Permutation Generator</ins>
- This program generates all permutations of numbers ```0``` through ```n-1``` (currently set to ```n=3```), using recursion. It was created as a class exercise to understand recursion and backtracking. Print statements are included throughout to show recursion depth and what happens at the end of each loop.

### <ins>Non-touching Diagonals</ins>
- This program creates an n x n board and attempts to fill in sqaures with diagonals ```\``` or ```/``` (or leave them empty) without letting the endpoints of the diagonals touch. The goals of the program is to search for solutions that create a board of a given size with a given number of diagonals. The program will continue to run until all permutations are tried, and a list of all solutions will be printed. Again, print statements are included throughout to show recursion depth and each step through loops. This program slows down significantly for n>3, so I plan to refactor in order to speed up processing.
- Note: In this program, `\` diagonals are represented by 1s, and `/` diagonals are represented by 2s. Empty squares are represented by 0s.
