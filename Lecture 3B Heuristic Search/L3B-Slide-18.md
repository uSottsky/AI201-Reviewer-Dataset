# Properties of A* Complexity

Heuristic Accuracy and Search Performance

Let N be the total number of nodes expanded by $A^{*}$ and the solution depth is d.
The effective branching factor, $b^{*}$, is the branching factor that a uniform tree of depth d would have to have in order to contain N nodes, i.e.

					$N=1+b^{*}+(b^{*})^{2}+...+(b^{*})^{d}$

• the effective branching factor for a given heuristic is fairly constant over a wide range of problem instances
• a very good heuristic would have a $b^{*}$ close to 1.0
• for the 8-puzzle example above, for any node n, $h_{2}(n)\ge h_{1}(n)$ We say that $h_{2}$ dominates $h_{1}$

18/25

---
**Navigation** [[L3B-Slide-17|Previous ← Heuristic Functions for N-Puzzle]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-19|Next → Search Cost Comparison]]