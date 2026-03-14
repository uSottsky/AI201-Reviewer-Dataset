# Monte Carlo Tree Search (MCTS)

![[Pasted image 20260315010005.png]]
> Reference: Slide 29 - Three-part diagram illustrating MCTS steps: (a) Selection, (b) Expansion and simulation, (c) Backpropagation, showing nodes with fractions like (37/100) updating to (37/101) upon a "black wins" result.

MCTS maintains a search tree and grows it on each iteration of the following steps:
1. **Selection:** from root, choose a move (guided by selection policy) leading to a successor node and repeat the process, moving down the tree to a leaf
2. **Expansion:** grow the tree by generating a new child of the selected node
3. **Simulation:** perform a playout from the newly generated child node, choosing moves for both players according to the playout policy. These moves are not recorded in the search tree.
4. **Back-propagation:** use the results of the simulation to update all the search nodes going up to the root.

 
29/34

---
**Navigation**
[[L3C-Slide-28|Previous ← Pure Monte Carlo Search]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-30|Next → MCTS Pseudo-code]]