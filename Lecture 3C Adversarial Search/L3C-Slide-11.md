# Minimax Algorithm

![[Pasted image 20260315004854.png]]
> Reference: Slide 11 - A min-max tree showing MAX at the root (node A, value 3), MIN at the next level (nodes B, C, D), and terminal leaf nodes with values like 3, 12, 8, 2, 4, 6, 14, 5, 2.

1. Generate the entire game tree up to the terminal states.
2. Compute the pay-off of each terminal state using the utility function
3. Use the pay-off values of the terminal states to determine the pay-off values of the nodes one level higher up the search tree.
   * pay-off value for a higher level node is the lowest pay-off of the node's children if it is MIN's turn to move, or the highest pay-off if it is MAX's turn.
4. Continue backing up the values from the leaf nodes toward the root, one level at a time.
5. When the root node is reached, the branch that leads to the highest pay-off should be chosen by MAX

 
11/34

---
**Navigation**
[[L3C-Slide-10|Previous ← Minimax Optimal Strategy Equation]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-12|Next → Multiplayer Games]]