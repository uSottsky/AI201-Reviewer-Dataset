# Blind Search: Depth-Limited Search

### 4. Depth-Limited Search
* Depth-Limited Search is the same as DFS but with a cut-off on the maximum depth of a path.
* for the route finding example, there are 5 cities before reaching goal. The cut-off could be set to 4 steps.
* Depth-Limited search is complete (i.e. we are guaranteed to find solution) if depth limit > depth of solution.
* Depth-Limited search is not optimal for the same reason as DFS.
* Time complexity is $\mathcal{O}(b^{l})$ and space complexity is $\mathcal{O}(bl)$ for depth limit l.

35/41

---
**Navigation**
[[L3A-Slide-34|Previous ← DFS Storage & Completeness]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-36|Next → Iterative Deepening Search (IDS)]]