# Biological Neurons

![[Pasted image 20260316030243.png]]
> Reference: Slide 19 - Diagram of a Two-Layer Perceptron for solving XOR. The input layer ($x_1, x_2$) connects to a hidden layer of two neurons with specific weights and biases, which then connects to a single output neuron with its own weights and bias.

| $x_1$ | $x_2$ | $y_1$ | $y_2$ | $v$ | Output |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 0 | 0 | 0 | 0 | $(0 \cdot 1 + 0 \cdot -2) + (-1/2) = -1/2$ | 0 |
| 0 | 1 | 1 | 0 | $(1 \cdot 1 + 0 \cdot -2) + (-1/2) = 1/2$ | 1 |
| 1 | 0 | 1 | 0 | $(1 \cdot 1 + 0 \cdot -2) + (-1/2) = 1/2$ | 1 |
| 1 | 1 | 1 | 1 | $(1 \cdot 1 + 1 \cdot -2) + (-1/2) = -3/2$ | 0 |

* **Two-layer feedforward neural network**
* **Hidden layer:** first phase computations (input space to feature space transformation)
* **Output layer:** second phase computation (feature space)

---
**Navigation**
[[L7A-Slide-18|Previous ← Two-Layer Perceptron Mapping]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-20|Next → Network Architectures]]