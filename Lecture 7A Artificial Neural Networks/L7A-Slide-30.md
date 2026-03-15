# Biological Neurons

### Classification Capabilities of the 2 Layer Perceptron

![[Pasted image 20260316030739.png]]
> Reference: Slide 30 - Diagram of a 2 Layer Perceptron. Input nodes $x_1...x_l$ connect to hidden layer nodes $y_1...y_p$, which connect to a single output node.

Consider feature vectors $x \in \mathbb{R}^l$ and $p$ neurons in hidden layer. Assume one output neuron and step activation function.

Hidden layer neurons map input space onto vertices of hypercube of unit length in $p$-dimensional space, $H_p$:
$$H_p = \{[y_1, y_2, ..., y_p]^T \in \mathbb{R}^p, \ y_i \in [0, 1], \ 1 \le i \le p\}$$

* vertices of hypercube are points $[y_1, y_2, ..., y_p]^T$ of $H_p$ with $y_i \in \{0, 1\}$, $1 \le i \le p$
* mapping onto hypercube vertices achieved via creation of $p$ hyperplanes by $p$ neurons

---
**Navigation**
[[L7A-Slide-29|Previous ← Example: Character Recognition (Part 2)]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-31|Next → Example: Intersecting Hyperplanes in 2D]]