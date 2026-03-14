# Tree-structured CSP

>![[Pasted image 20260315015751.png]]
> Reference: Slide 25 - Linear ordering of the tree graph from A to F (A -> B -> C, D -> E, F).

### Algorithm for Tree-Structured CSP

1. Choose a variable as root, order variables from root to leaves such that every node's parent precedes it in the ordering.
2. For $j$ from $n$ down to $2$, apply `RemoveInconsistent(Parent(Xj), Xj)`
3. For $j$ from $1$ to $n$, assign $X_{j}$ consistently with `Parent(Xj)`

 
25/27

---
**Navigation**
[[L4-Slide-24|Previous ← Tree-Structured CSP]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-26|Next → Nearly Tree-Structured CSPs (Cutset)]]