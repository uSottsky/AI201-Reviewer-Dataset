# Blind Search: Uniform Cost Search

* UCS finds the cheapest solution if the cost of a path never decreases as we go along the path, i.e. $g(SUCCESSOR(n)) \ge g(n)$ for every node n.
* if every operator has a non-negative cost, then the cost of a path can never decrease as we go along the path.
* In this case, uniform cost search will find the cheapest path without exploring the whole search tree.
* Time and space complexity are both $\mathcal{O}(b^{d})$.

32/41

---
**Navigation**
[[L3A-Slide-31|Previous ← Uniform Cost Search (UCS)]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-33|Next → Depth-First Search (DFS)]]