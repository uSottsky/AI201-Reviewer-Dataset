# Perceptron

### The Perceptron


Once the Perceptron Algorithm has converged to a weight vector $w$ and a threshold $w_0$, classification of an unknown feature vector is performed via the perceptron rule:
* if $w^T x + w_0 \ge 0$ assign $x$ to $\omega_1$
* if $w^T x + w_0 < 0$ assign $x$ to $\omega_2$

**Network implementation:**



![[Pasted image 20260315215117.png]]
> Reference: Slide 17 - Diagrams of a Perceptron neural network model. (a) Shows a linear combiner explicitly followed by an activation function $f$. (b) Merges the combiner and activation function into a single node.


* In this neural model, a linear combiner is followed by the activation function (Fig. a). The combiner and activation function are merged together in Fig. b.
* feature vector elements $x_1, x_2, ..., x_l$ are applied to the input nodes of the network and each input multiplied by the corresponding weights $w_i, i=1,2,...l$. These are the synaptic weights of the network.
* The products are summed up together with the threshold $w_0$.
* The result goes through a nonlinear device that implements the activation function that outputs two possible values, -1 and +1 or 0 and 1.

---
**Navigation**
[[L6A-Slide-16|Previous ← Variant of the Perceptron Algorithm]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-18|Next → The Pocket Algorithm]]