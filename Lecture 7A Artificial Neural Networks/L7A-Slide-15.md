# Biological Neurons

### Perceptron realization of OR Gate

![[Pasted image 20260316030051.png]]
> Reference: Slide 15 - Diagram of a single perceptron for an OR gate with inputs $x_1$ and $x_2$, both with weights of 1, and a bias of $-1/2$.

activation function (step function):
$$f(v) = \begin{cases} 0 & \text{if } v < 0 \\ 1 & \text{if } v \ge 0 \end{cases}$$

| $x_1$ | $x_2$ | OR Class | $v$ | Output |
| :--- | :--- | :--- | :--- | :--- |
| 0 | 0 | B | $(0 \cdot 1 + 0 \cdot 1) + (-1/2) = -1/2$ | 0 |
| 0 | 1 | A | $(0 \cdot 1 + 1 \cdot 1) + (-1/2) = 1/2$ | 1 |
| 1 | 0 | A | $(1 \cdot 1 + 0 \cdot 1) + (-1/2) = 1/2$ | 1 |
| 1 | 1 | A | $(1 \cdot 1 + 1 \cdot 1) + (-1/2) = 3/2$ | 1 |

---
**Navigation**
[[L7A-Slide-14|Previous ← The AND and OR Gates]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-16|Next → The XOR Problem]]