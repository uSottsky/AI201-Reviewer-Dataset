# Conventions and Notations

![[Pasted image 20260314203430.png]]
> Reference: Slide 12 - Diagram showing neurons i, j, and k with their respective weights $w_{ji}(n)$ and $w_{kj}(n)$ and outputs $y_i(n)$ and $y_j(n)$.

### Conventions and Notations
* function signals move from left to right and error signals from right to left.
* iteration $n$ refers to the $n$-th training pattern presented to the network.
* neuron $i$ lies to the left of neuron $j$ and is connected to neuron $j$.
* neuron $k$ lies to the right of neuron $j$ and is connected to neuron $j$.
* weight connecting the output of neuron $i$ to the input of neuron $j$ at iteration $n$ is denoted by $w_{ji}(n)$.
* weight connecting the output of neuron $j$ to the input of neuron $k$ at iteration n is denoted by $w_{kj}(n)$.
* $y_{i}(n)$ is the output of neuron $i$ and one of the inputs of neuron $j$


12/39

---
**Navigation**
[[L7B-Slide-11|Previous ← BP Derivation Output vs Hidden]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-13|Next → Output Neuron Error]]