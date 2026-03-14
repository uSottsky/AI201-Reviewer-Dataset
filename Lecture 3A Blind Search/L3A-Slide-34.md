# Blind Search: Depth-First Search

* stores path from root to leaf node and all remaining unexpanded sibling nodes for each node on the path
* for branching factor b and maximum depth of search tree m, the required storage is $b^{m}$ nodes
* time complexity of DFS is $\mathcal{O}(b^{m})$ but on the average it performs better than BFS since BFS looks at all nodes on depth $d-1$ before going to nodes on depth d
* DFS may never terminate if the tree is of infinite depth (it would just keep on expanding nodes forever).
* DFS could also return a solution path that is longer than the optimal solution since it could find a deep solution even when a shallow solution exists.
* DFS is neither complete nor optimal. We must avoid using DFS for search trees with large or infinite maximum depths.

34/41

---
**Navigation**
[[L3A-Slide-33|Previous ← Depth-First Search (DFS)]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-35|Next → Depth-Limited Search]]