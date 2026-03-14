# Monte Carlo Tree Search (MCTS)

### Go
* branching factor is very large (> 360) which limits Alpha-Beta Pruning to 4 to 5 ply
* difficult to define a good evaluation function for Go
  * material value is not a good indicator
  * most positions are in flux until the endgame

**Monte Carlo Tree Search (MCTS)** - instead of a heuristic evaluation function, value of a state is estimated as the average utility over a number of simulations of complete games starting from the state
* a simulation (or playout) chooses moves first for one player and for the other until the terminal position is reached
* moves are chosen randomly during playout but a **playout policy** biases the moves towards good ones
* playout policy learned from self-play using neural networks

 
27/34

---
**Navigation**
[[L3C-Slide-26|Previous ← Game of Go]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-28|Next → Pure Monte Carlo Search]]