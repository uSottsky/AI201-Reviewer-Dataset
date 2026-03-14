# Heuristic Alpha-Beta Tree Search

### Forward Pruning
Alpha-Beta Pruning prunes any node that is provably outside the current $\alpha-\beta$ window.

**Probabilistic Cut (ProbCut)** - forward pruning version of Alpha-Beta Pruning that prunes nodes that are probably outside the window.
* probability computed through a shallow search to compute the backed-up value of a node and using past experience to estimate how likely it is that the node's score is outside the $\alpha-\beta$ window.

### Look up table for opening and end games
* **openings** - rely on human experts (e.g., Sicilian, French, Ruy-Lopez, etc)
* **ending** - rules for king-and-rook-vs-king (KRK), king-bishop-knight-vs-king (KBNK)
* tables could have 400 trillion entries for KBNK endings

 
25/34

---
**Navigation**
[[L3C-Slide-24|Previous ← Quiescence and Singular Extension]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-26|Next → Game of Go]]