# Heuristic Alpha-Beta Tree Search

### Chess
* Average branching factor: 35
* up to 50 moves $\rightarrow$ $35^{100}$ nodes to consider

### Evaluation Functions for Chess
* material value + good positional features
* assign a material value to each piece:
  * pawn: 1
  * knight/bishop: 3
  * rook: 5
  * queen: 9
* "good pawn structure" (use a pawn to defend another pawn): 0.5
* "isolated pawn" (no pawns on adjacent files): $-1/3$
* "control of center of board"
* "how well protected is the king"

 
20/34

---
**Navigation**
[[L3C-Slide-19|Previous ← Heuristic Alpha-Beta Tree Search]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-21|Next → Linear vs Non-linear Evaluation]]