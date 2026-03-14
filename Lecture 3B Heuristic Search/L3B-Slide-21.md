# $A^{*}$ Pseudo-code

$A^{*}$ Pseudo-code
does not build an actual tree-like structure instead uses a list called OPEN, containing nodes ready for expansion, and another list called CLOSED containing expanded nodes.

1. Put the start node s on a list called OPEN and compute $f(s)$.
2. If OPEN is empty, exit with failure; otherwise continue.
3. Remove from OPEN that node whose f value is smallest and put it on a list called CLOSED. Call this node n. (Resolve ties for minimal f values arbitrarily, but always in favor of any goal node.)
4. If n is a goal node, exit with the solution path obtained by tracing back the pointers; otherwise continue.
5. Expand node n, generating all of its successors. If there are no successors, go immediately to 2. For each successor $n_{i}$, compute $f(n_{i})$.
6. Associate with the successors not already on either OPEN or CLOSED the f values just computed. Put these nodes on OPEN and direct pointers from them back to n.
7. Associate with those successors that were already on OPEN or CLOSED the smaller of the f values just computed and their previous f values. Put on OPEN those successors on CLOSED whose f values were thus lowered, and redirect to n the pointers from all nodes whose f values were lowered.
8. 8Go to 2.

Comments:
• duplicates are not retained; when nodes are rediscovered, the ancestor history is updated
• when a successor is already on OPEN or CLOSED, the algorithm modifies the pointers so that the nodes record the shorter of the two partial paths

21/25

---
**Navigation** [[L3B-Slide-20|Previous ← Multiple Heuristics]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-22|Next → Memory Bounded Search]]