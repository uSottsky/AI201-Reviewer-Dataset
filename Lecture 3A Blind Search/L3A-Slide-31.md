# Blind Search: Uniform Cost Search

### 2. Uniform Cost Search (Dijkstra, 1959)
* **UCS** - similar to the BFS except that it always expands the lowest-cost node on the fringe (as measured by the path cost $g(n)$), rather than the lowest-depth node.
* In fact, BFS is just a special case of uniform cost search with $g(n) = DEPTH(n)$.

![[Pasted image 20260314134531.png]]
> Reference: Slide 31 - Step-by-step route finding search trees (a) and (b) with path costs labeled.

* Provided that certain conditions are met, the first solution that is found is guaranteed to be the cheapest solution since if there were a cheaper path that was a solution, it would have been expanded earlier, and therefore would have been found first.

31/41

---
**Navigation**
[[L3A-Slide-30|Previous ← BFS Time & Memory Requirements]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-32|Next → UCS Costs & Complexity]]