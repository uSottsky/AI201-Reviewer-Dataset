# A* Search

If the $h(n)$ is less than the actual distance from node n to goal, then it is called an admissible heuristic.
- if h is admissible, $f(n)$ never overestimates the actual cost of the best solution through node n.

Among algorithms that extend search paths from the root, $A^{*}$ is optimally efficient for any given heuristic function.
- no other optimal algorithm is guaranteed to expand fewer nodes than $A^{*}$ (Dechter and Pearl, 1983).

11/25

---
**Navigation** [[L3B-Slide-10|Previous ← A* Search]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-12|Next → A* Solution Route Finding]]