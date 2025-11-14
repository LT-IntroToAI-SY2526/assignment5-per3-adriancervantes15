# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

The major thing that I learned in this assignment was the new search algorithims. I had heard of them before but did not really go deep into them. One particular challenge that I faced in this assignment was the concept of backtracking. But now I know that backtracking only works with DFS because DFS goes through a path as far as possible, while bfs doesn't.

2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

I think one future project where I would either use BFS or DFS would be a maze-type of problem. Since a maze has several paths that lead into deadends, I think that DFS would be a good use as it would explore a path until it reached the solution or a deadend. If it found a dead end it would backtrack and start again. 


3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

Stack classes work by removing the last element that was added, first. Queue classes work by removing the first element added. They are imporntat for algorithims, as they either help go deeper into a part, or go level by level going searching through everything. A stack changes the way the search algorithim explores possible solutions as it goes as deep as it can into one possiblity. A queue is better for a BFS algorithim as it 