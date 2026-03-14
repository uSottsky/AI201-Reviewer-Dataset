# Properties of A* Complexity

The following table:

| d | BFS | $A^{*}(h_{1})$ | $A^{*}(h_{2})$ | BFS | $A^{*}(h_{1})$ | $A^{*}(h_{2})$ |
|---|---|---|---|---|---|---|
| 6 | 128 | 24 | 19 | 2.01 | 1.42 | 1.34 |
| 8 | 368 | 48 | 31 | 1.91 | 1.40 | 1.30 |
| 10 | 1033 | 116 | 48 | 1.85 | 1.43 | 1.27 |
| 12 | 2672 | 279 | 84 | 1.80 | 1.45 | 1.28 |
| 14 | 6783 | 678 | 174 | 1.77 | 1.47 | 1.31 |
| 16 | 17270 | 1683 | 364 | 1.74 | 1.48 | 1.32 |
| 18 | 41558 | 4102 | 751 | 1.72 | 1.49 | 1.34 |
| 20 | 91493 | 9905 | 1318 | 1.69 | 1.50 | 1.34 |
| 22 | 175921 | 22955 | 2548 | 1.66 | 1.50 | 1.34 |
| 24 | 290082 | 53039 | 5733 | 1.62 | 1.50 | 1.36 |
| 26 | 395355 | 110372 | 10080 | 1.58 | 1.50 | 1.35 |
| 28 | 463234 | 202565 | 22055 | 1.53 | 1.49 | 1.36 |

Figure 3.26 Comparison of the search costs and effective branching factors for 8-puzzle problems using breadth-first search, $A^{*}$ with $h_{1}$ (misplaced tiles), and $A^{*}$ with $h_{2}$ (Manhattan distance).
Data are averaged over 100 puzzles for each solution length d from 6 to 28.

 19/25

---
**Navigation** [[L3B-Slide-18|Previous ← Heuristic Accuracy]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-20|Next → Multiple Heuristics]]