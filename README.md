# Recursive programs
This repository started with a permutation generator, and now contains several other Python programs created from class exercises that use recursion and backtracking.

### <ins>Permutation Generator</ins>
- This program generates all permutations of numbers ```0``` through ```n-1``` (currently set to ```n=3```), using recursion. It was created as a class exercise to understand recursion and backtracking. Print statements are included throughout to show recursion depth and what happens at the end of each loop.

### <ins>Non-touching Diagonals</ins>
- This program creates an n x n board and attempts to fill in sqaures with diagonals ```\``` or ```/``` (or leave them empty) without letting the endpoints of the diagonals touch. The goals of the program is to search for solutions that create a board of a given size with a given number of diagonals. The program will continue to run until all permutations are tried, and a list of all solutions will be printed. Print statements are included throughout to show recursion depth and each step through loops. This program slows down significantly for n>3, so further refactoring is planned.
- Note: In this program, `\` diagonals are represented by 1s, and `/` diagonals are represented by 2s. Empty squares are represented by 0s.

### <ins>Non-touching Diagonals Var1</ins>
- This version of the above program improves speed by removing print statements, which resulted in a significant performance improvement. This one change improved performance more than the attempt to cut down recursive iterations by exiting known bad pathways.
- Also added to this program is a function to print the solutions as `\` ` ` `/` instead of numbers.

### <ins>Non-touching Diagonals Var2</ins>
- This version represents the board as a flat array, rather than nested arrays of rows. This improved performance further, and simplified debugging due to more straightforward indexing.
- This prorgam also represents the diagonals with `\` ` ` `/` instead of numbers.

## Key Learnings
- Recursing and backtracking can be applied to quickly map out complex search problems.
- Each level of a recursively called function maintains its own local variables.
- One must be careful when manipulating indexing variables passed as arguments in the function. 
- A surprising insight was how expensive print statements are, and how removing them lead to more significant performance improvement that even optimizing the recursion itself.
- A flat array representation can also lead to performance improvements compared to nested arrays.
