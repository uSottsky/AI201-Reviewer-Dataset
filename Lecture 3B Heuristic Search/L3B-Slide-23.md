# Iterative Deepening $A^{*}$ (Korf)


a modification of $A^{*}$ that reduces its space complexity from exponential to linear
- performs a series of depth-first searches in which a branch is cut off when the cost of its frontier node, $f(n)=g(n)+h(n)$, exceeds a cutoff threshold
- threshold starts at the heuristic estimate of the initial state, and is increased each iteration to the minimum value that exceeded the previous threshold, until a solution is found.

Both $A^{*}$ and $IDA^{*}$ have exponential time complexities.
IDA* uses space that is proportional to the longest path it explores since it is depth-first.
- can solve the 15-puzzle but not the 24-puzzle
- storage requirement is about bd nodes

23/25

---
**Navigation** [[L3B-Slide-22|Previous ← Memory Bounded Search]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-24|Next → IDA* Algorithm]]