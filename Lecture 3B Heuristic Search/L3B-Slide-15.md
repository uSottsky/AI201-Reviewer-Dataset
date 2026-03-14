# Properties of A* Completeness

Proof of the Completeness of $A^{*}$

Since $A^{*}$ expands nodes of increasing $f$, ($f$ is increasing towards $f*$), it will eventually reach a goal state.

This is true unless there are infinitely many nodes with $f(n)<f^{*}(n)$. There is an infinite number of nodes when
- there is a node with an infinite branching factor
- there is a path with a finite path cost but an infinite number of nodes along it

$A^{*}$ is complete on locally finite graphs (graphs with a finite branching factor) provided there is some positive constant such that every operator costs at least δ.

15/25

---
**Navigation** [[L3B-Slide-14|Previous ← Monotonicity]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-16|Next → Complexity]]