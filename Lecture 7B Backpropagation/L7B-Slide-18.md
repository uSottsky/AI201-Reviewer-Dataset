# Backpropagation Algorithm Derivation

Backpropagation Algorithm: weight adjustment is proportional to the gradient at the error surface
# $\Delta w_{ji}(n)=-\eta\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}$
# $=+\eta e_{j}(n)\varphi^{\prime}(v_{j}(n))y_{i}(n)$
# $=\eta\delta_{j}(n)y_{i}(n)$


where $\delta_{j}(n)$ is the **local gradient** defined as

# $\delta_{j}(n)=-\frac{\partial\mathcal{E}(n)}{\partial e_{j}(n)}\frac{\partial e_{j}(n)}{\partial y_{j}(n)}\frac{\partial y_{j}(n)}{\partial v_{j}(n)}$
# $\delta_{j}(n)=e_{j}(n)\varphi^{\prime}(v_{j}(n))$                                                      (11)


18/39

---
**Navigation**
[[L7B-Slide-17|Previous ← Chain Rule Derivation]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-19|Next → Case 2: Hidden Neuron]]