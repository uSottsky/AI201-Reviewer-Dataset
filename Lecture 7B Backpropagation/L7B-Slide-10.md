# Backpropagation Algorithm Derivation

![[Pasted image 20260314203308.png]]
> Reference: Slide 10 - Diagram illustrating the forward propagation of function signals (solid arrows) and backward propagation of error signals (dashed arrows) through a node.

### Two types of signal flows in a MLP
1. **forward propagation of function signals**
    * function signals come in at the network inputs, get modified as they pass through the network, and emerge as output signals.
2. **backward propagation of error signals**
    * error signals come from the output neurons and propagate backward through the network.
    * error signals are used to adjust the weights of the individual neurons

* MLP uses a smooth (differentiable) activation function
* activation function must be nonlinear, otherwise MLP is just equivalent to a single-layer perceptron

10/39

---
**Navigation**
[[L7B-Slide-09|Previous ← History of Backpropagation]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-11|Next → BP Derivation Output vs Hidden]]