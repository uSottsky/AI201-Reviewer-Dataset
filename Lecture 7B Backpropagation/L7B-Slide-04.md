# Model of a Neuron
![[Pasted image 20260314202250.png]]

> Reference: Slide 4 - Diagram of the mathematical neuron model and a graph showing the affine transformation of the induced local field with bias $b_k$.

For a neuron k,
# $u_{k}=\sum_{j=1}^{m}w_{kj}x_{j}$                                                             (1)
# $y_{k}=\varphi(u_{k}-b_{k})$                                                               (2)

where
* $x_{1},x_{2},...x_{m}$ are the input signals
* $w_{k1},w_{k2},...w_{km}$ are the synaptic weights
* $b_{k}$ is the bias
* $\varphi(\cdot)$ is the activation function
* $u_{k}-b_{k}$ is the internal activity 
* $y_{k}$ is the output
* bias applies an affine transformation to output $u_{k}$
![[Pasted image 20260314202442.png]]

4/39

---
**Navigation**
[[L7B-Slide-03|Previous ← Model of a Neuron]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-05|Next → Neuron Model with Bias Input]]