# Decision Rule

For a trained MLP, how do we decide which class a pattern belongs to ?

Assign vector x in a particular class k if the corresponding output value $y_{k}$ is larger than some fixed threshold (e.g. 0.5).
* could lead to multiple class assignments

Let $F(\cdot)$ be the mapping function learned by the network that maps the input to its output and let $F_{k}(x)$ be the output of the network for input x.
Assume that the network is trained with binary target values.
The most appropriate output decision rule is as follows:
Classify the vector x as belonging to class $C_{k}$ if
$F_{k}(x)\ge F_{j}(x)$
for all $j\ne k$

where $F_{k}(x)$ and $F_{j}(x)$ are the function values for the mapping function $F(x)$.

34/39

---
**Navigation**
[[L7B-Slide-33|Previous ← Other Heuristics]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-35|Next → Convergence]]