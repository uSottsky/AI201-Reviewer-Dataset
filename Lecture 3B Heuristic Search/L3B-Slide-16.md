# Properties of A* Complexity

Complexity of $A^{*}$

It can be shown that $A^{*}$ is of exponential complexity unless the error in the heuristic function grows no faster than the logarithm of the actual path cost, i.e.
						$|h(n)-h^{*}(n)|\le O(log~h^{*})$
where $h^{*}(n)$ is the true cost from node n to the goal.

Memory space, more than computation time, is $A^{*}$'s main drawback.

16/25

---
**Navigation** [[L3B-Slide-15|Previous ← Completeness]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-17|Next → Heuristic Functions for N-Puzzle]]