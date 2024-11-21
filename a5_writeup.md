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

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
Compared to the breadth-first search, I thought the depth-first serch was more efficient as it tended to solve the puzzle with fewer iterations. However, despite this, the computer does it so quickly that for the purpose of a 9x9 sudoku board it didn't really matter, but if it was a huge board it would be better to use DFS. 


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
The choice of data structures didn't really impacted the functionality of the algorithm so much as it impacted the speed of solving the puzzle. I don't personally know about any alternative data structures that could have been used to achieve the same objective, but I did prefer the setup of the stack compared to the queue. I know about using things like 2D arrays from CSA which reminded me of the stacks and queues but I don't think they are as useful in comparison. I read a bit about sets and those might be helpful for hard games because it could help with keeping track of the possibilities for each box as they go along similar to how a human would do it if they were solving it. I honestly think what we used served its purpose well though for this objective.    


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
Considering the current implementation, the Sudoku solver could be adapted for larger puzzles because we could just change the board size or grid-size to accomodate. I think the overall lesson from doing this assignment was understanding that even though we used things like DFS and BFS and the sudoku class for the pupose of this assignment alone, the guiding principles and functions we used could be applied for other things too (assuming it was done right). Although we completed the assignment for the sake of this assignment, we can carry over those skills to other projects in the future. 