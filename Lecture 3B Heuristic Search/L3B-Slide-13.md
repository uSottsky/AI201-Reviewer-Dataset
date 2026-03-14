# Properties of A* Optimality

Proof of the Optimality of $A^{*}$

Recall:
							$f(n)=g(n)+h(n)$
 - $g(n)$ is path cost from start node to node n
 - $h(n)$ is estimated cost of the cheapest path from n to goal

![[Pasted image 20260314150706.png]]
Let G be an optimal goal state whose path cost is $f^{*}$ and let $G_{2}$ be a suboptimal goal state.
The path cost is therefore
							$g(G_{2})>f^{*}$

Consider a node n that is currently a leaf node on an optimal path to G. Since h is admissible, then $f^{*}\ge f(n)$.

If n is not chosen for expansion over $G_{2}$, then $f(n)\ge f(G_{2})$ so that
							$f^{*}\ge f(G_{2})$

However, since $G_{2}$ is a goal state, we have $h(G_{2})=0$ and therefore $f(G_{2})=g(G_{2})$. Thus,
							$f^{*}\ge g(G_{2})$  (2)

which contradicts our previous assumption (1).

We therefore conclude that $A^{*}$ never reaches a suboptimal goal. Q.E.D.


Heuristic Search 13/25

---
**Navigation**
[[L3B-Slide-12|Previous ← A* Solution Route Finding]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-14|Next → Monotonicity]]