# What is CSP?

A Constraint Satisfaction Problem consists of the three components, X, D, and C:
* **X**: set of variables $\{X_{1},...,X_{n}\}$
* **D**: set of domains $\{D_{1},...,D_{n}\}$, one for each variable
* **C**: set of constraints that specify allowable combinations of values

A domain $D_{i}$ consists of a set of allowable values $\{v_{1},...,v_{k}\}$ for each variable $X_{i}$.
* Boolean variable has domain ${true, false}$
* different variables can have different domains of different sizes

Each constraint $C_{j}$ consists of a pair $(scope, rel)$ where
* **$scope$**: tuple of variables that participate in the constraint
* **$rel$: is a relation that defines the values that the variables can take on

A relation can be represented as:
* an explicit set of tuples of values that satisfy the constraint, or
* a function that can compute whether a tuple is a member of the relation

If $X_{1}$, $X_{2}$ have domains {1, 2, 3}, the constraint that $X_{1}$ must be greater than $X_{2}$ is written:
* $(((X_{1}, X_{2}), \{(3, 1), (3, 2), (2, 1)\}))$
* $(((X_{1}, X_{2}), X_{1} > X_{2}))$

 
4/27

---
**Navigation**
[[L4-Slide-03|Previous ← What is CSP?]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-05|Next → Assignments & Solutions]]