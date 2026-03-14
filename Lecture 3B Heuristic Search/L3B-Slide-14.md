# Admissible Heuristics and Monotonicity


Most admissible heuristic functions are monotonic, i.e. they make the resulting f-cost non-decreasing along any path from the root.

If an admissible heuristic is not monotonic, we modify f to make it monotonic.

Consider two nodes $n$ and $n^{\prime}$, where n is the parent of $n^{\prime}$.
Suppose $f(n)>f(n^{\prime})$, i.e., we have a nonmonotonic heuristic. Observe that any path through $n^{\prime}$ is also a path through n.

The value $f(n^{\prime})$ can be disregarded since we know that the path cost is at least $f(n)$.

We then modify f as follows:

				$f(n^{\prime})=max(f(n),g(n^{\prime})+h(n^{\prime}))$

i.e., we check the f-cost of a new node to see if it is less than its parent's.
If it is so, then we use the parent's f-cost instead.
This is the **path max** equation.

14/25

---
**Navigation**
[[L3B-Slide-13|Previous ← Proof of Optimality]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-15|Next → Completeness]]