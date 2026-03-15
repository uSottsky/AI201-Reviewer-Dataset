# The Multi-layer Perceptron

### Universal Approximation Theorem
**Universal Approximation Theorem (Cybenko, 1989; Hornik, 1991)**

Let $\sigma : \mathbb{R} \rightarrow \mathbb{R}$ be a nonconstant, bounded, and continuous function and let $I_m$ denote the $m$-dimensional unit hypercube $[0,1]^m$.

The space of real-valued continuous functions on $I_m$ is denoted by $C(I_m)$.
Then, given any $\epsilon > 0$ and any function $f \in C(I_m)$, there exists an integer $N$, real constants $v_i, b_i \in \mathbb{R}$ and real vectors $w_i \in \mathbb{R}^m$ for $i=1,...,N$ such that we may define:
$$F(x) = \sum_{i=1}^N v_i \sigma(w_i^T x + b_i)$$
as an approximate realization of the function $f$, that is,
$$|F(x) - f(x)| < \epsilon$$
for all $x \in I_m$.

A two-layer neural network can approximate arbitrary continuous functions arbitrarily well, provided that the hidden layer is sufficiently wide.

---
**Navigation**
[[L7A-Slide-35|Previous ← Representational Power of Feedforward Networks]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-37|Next → References]]