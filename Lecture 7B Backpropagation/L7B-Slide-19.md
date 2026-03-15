# Backpropagation Algorithm Derivation

### Case 2: Hidden Neuron

![[Pasted image 20260314211521.png]]
> Reference: Slide 19 - Diagram showing connection from node i to hidden node j to output node k.

For hidden neurons,
* no desired response signal that can be used to adjust the weights
* error signal computed recursively in terms of the error signals of all the neurons to which the hidden neuron is directly connected

For hidden neuron **$j$**
# $\delta_{j}(n)=-\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}\frac{\partial y_{j}(n)}{\partial v_{j}(n)}$
# $=-\frac{\partial\mathcal{E}(n)}{\partial y_{j}(n)}\varphi^{\prime}(v_{j}(n))$


What is $\partial\mathcal{E}(n)/\partial y_{j}(n)$?

19/39

---
**Navigation**
[[L7B-Slide-18|Previous ← Local Gradient (Delta)]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-20|Next → Hidden Neuron Error Gradient]]