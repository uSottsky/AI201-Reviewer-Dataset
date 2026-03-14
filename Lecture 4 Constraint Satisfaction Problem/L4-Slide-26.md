#  Nearly tree-structured CSPs

**Conditioning:** instantiate a variable, prune its neighbors' domains.

> ![[Pasted image 20260315015840.png]]
> Reference: Slide 26 - Diagram demonstrating Cutset Conditioning on the Australia map. Node 'SA' is instantiated, removing it and its edges to turn the remaining cyclic graph into a tree.

**Cutset conditioning:** instantiate (in all ways) a set of variables such that the remaining constraint graph is a (residual) tree with restricted domain.

**Cutset size:** runtime $O(d^{c} \cdot (n-c)d^{2})$, very fast for small $c$.

 
26/27

---
**Navigation**
[[L4-Slide-25|Previous ← Algorithm for Tree-Structured CSP]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-27|Next → End]]