# Backpropagation Algorithm Derivation

Finally, we have the Delta Rule
# $\Delta w_{ji}(n)=\eta\delta_{j}(n)y_{i}(n)$

where
# $\delta_{j}(n)=e_{j}(n)\varphi^{\prime}(v_{j}(n))$ if neuron $j$ is an output neuron
and
# $\delta_{j}(n)=\varphi^{\prime}(v_{j}(n))\sum_{k}\delta_{k}(n)w_{kj}(n)$ if neuron $j$ is a hidden neuron

The local gradient $\delta_{j}(n)$ depends on whether neuron $j$ is an output neuron or hidden neuron:
* neuron $j$ is an output neuron: $\delta_{j}(n)$ is the product of the derivative $\varphi^{\prime}(v_{j}(n))$ and the error signal $e_{j}(n)$
* neuron $j$ is a hidden neuron: $\delta_{j}(n)$ is the product of the derivative $\varphi^{\prime}(v_{j}(n))$ and the weighted sum of the $\delta$'s computed for the neurons in the forward layer that is connected to neuron $j$


22/39

---
**Navigation**
[[L7B-Slide-21|Previous ← Hidden Neuron Delta]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-23|Next → Logistic Function Nonlinearity]]