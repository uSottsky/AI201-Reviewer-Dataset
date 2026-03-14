# Backpropagation Algorithm Derivation

### Output Neuron

![[Pasted image 20260314203903.png]]
> Reference: Slide 15 - Diagram of output neuron j (same as Slide 13).

For inputs $[+1,y_{1}(n),...y_{i}(n),y_{p}(n)]$, the net internal activity for output neuron $j$ is
				
# $v_{j}(n)=\sum_{i=0}^{p}w_{ji}(n)y_{i}(n)$                                                       (7)

where p is the number of neurons in the previous layer.
the synaptic weight $w_{j0}$ corresponding to a fixed input $y_{0}=+1$ is the bias $b_{j}$ for neuron $j$.

The neuron's output signal is
# $y_{j}(n)=\varphi(v_{j}(n))$                                                                     (8)


15/39

---
**Navigation**
[[L7B-Slide-14|Previous ← Cost Function (Error)]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-16|Next → BP Instantaneous Gradient]]