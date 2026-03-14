# What is CSP?

* Finite domain of size d in n variables: $O(d^{n})$ possible assignments.
* An assignment $\{X_{1}=v_{1}, X_{2}=v_{2}, ...\}$ that does not violate any constraint is called a **consistent** or legal assignment.
* A **complete assignment** is one in which every variable is assigned a value.
* A **solution** to a CSP is a consistent, complete assignment.
* A **partial assignment** is one that leaves some variables unassigned, and a partial solution is a partial assignment that is consistent.

In general, solving a CSP is an NP-complete problem, although there are subclasses of CSPs that can be solved very efficiently.

 
5/27

---
**Navigation**
[[L4-Slide-04|Previous ← CSP Components (X, D, C)]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-06|Next → Example: Map Coloring]]