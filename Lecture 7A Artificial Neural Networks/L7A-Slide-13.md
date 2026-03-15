# Model of a Neuron
![[Pasted image 20260316025531.png]]

![[Pasted image 20260316025959.png]]
> Reference: Slide 13 - Diagram of an artificial neuron model showing input signals ($x_1 ... x_m$) multiplied by synaptic weights ($w_{k1} ... w_{km}$), feeding into a Summing junction $\Sigma$ along with a Bias $b_k$. The output $v_k$ passes through an Activation function $\varphi(\cdot)$ to produce Output $y_k$.

**Elements:**
* **synapses** - represented by connecting links, each characterized by a weight
  * positive/negative weight values $\rightarrow$ excitatory/inhibitory synapse
  * inputs are multiplied by weights to yield weighted inputs
* **summer** - sums up the weighted inputs
* **activation function** - limits the amplitude of the output to avoid saturation
  * also called the "squashing function"
  * normalizes the amplitude range of the output to $[0, 1]$ or $[-1, 1]$

---
**Navigation**
[[L7A-Slide-12|Previous ← Short History of ANN]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-14|Next → The AND and OR Gates]]