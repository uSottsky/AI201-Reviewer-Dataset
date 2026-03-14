# Blind Search: Breadth-First Search

* BFS is implemented by calling the GENERAL-SEARCH algorithm with a queuing function that puts newly generated states at the end of the queue.
* If there is a solution, BFS is guaranteed to find it (BFS is complete).
* If there are several solutions, the shallowest goal will always be found.
* It is optimal provided the path cost is a nondecreasing function of the depth of the node.
* If each expansion yields b new states, we say that the branching factor of the tree is b.
* If the goal node is found at depth d, the maximum number of nodes expanded before finding a solution is $1 + b + b^{2} + b^{3} + ... b^{d}$.

29/41

---
**Navigation**
[[L3A-Slide-28|Previous ← Breadth-First Search (BFS)]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-30|Next → BFS Time & Memory Requirements]]