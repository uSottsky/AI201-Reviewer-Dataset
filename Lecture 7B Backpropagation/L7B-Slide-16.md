# Backpropagation Algorithm Derivation

### Output Neuron
Backpropagation algorithm: the weight adjustment is proportional to the instantaneous gradient:

# $\Delta w_{ji}(n)=-\eta\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}$                                                               (9)

where the gradient is
# $\frac{\partial\mathcal{E}(n)}{\partial w_{ji}(n)}=\frac{\partial\mathcal{E}(n)}{\partial e_{j}(n)}\frac{\partial e_{j}(n)}{\partial y_{j}(n)}\frac{\partial y_{j}(n)}{\partial v_{j}(n)}\frac{\partial v_{j}(n)}{\partial w_{ji}(n)}$


16/39

---
**Navigation**
[[L7B-Slide-15|Previous ← Output Neuron Activation]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-17|Next → Chain Rule Derivation]]