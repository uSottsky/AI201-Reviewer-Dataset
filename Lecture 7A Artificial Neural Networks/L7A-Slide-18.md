# Biological Neurons

![[Pasted image 20260316030224.png]]
> Reference: Slide 18 - Two side-by-side graphs. Left: the input space ($x_1, x_2$) with two decision lines. Right: the feature space ($y_1, y_2$) where the problem has become linearly separable with a single new decision line.

| $x_1$ | $x_2$ | 1st Phase $y_1$ | 1st Phase $y_2$ | 2nd Phase |
| :--- | :--- | :--- | :--- | :--- |
| 0 | 0 | $0(-)$ | $0(-)$ | B (0) |
| 0 | 1 | $1(+)$ | $0(-)$ | A (1) |
| 1 | 0 | $1(+)$ | $0(-)$ | A (1) |
| 1 | 1 | $1(+)$ | $1(+)$ | B (0) |

* **Phase 1:** map input vector to new vector $y=[y_1, y_2]^T$
  * 2 lines defined 3 regions $(00, 10, 11)$
* **Phase 2:** separate $[y_1, y_2]=[0, 0]$ and $[y_1, y_2]=[1, 1]$ (Class B) from $[y_1, y_2]=[1, 0]$ (Class A)
  * use a 3rd neuron for this

Mapping of the first phase transforms the nonlinearly separable problem into a linearly separable one.

---
**Navigation**
[[L7A-Slide-17|Previous ← The Two-Layer Perceptron]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-19|Next → Two-Layer Perceptron Network Diagram]]