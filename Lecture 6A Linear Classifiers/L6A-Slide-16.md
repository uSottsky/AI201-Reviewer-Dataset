# Perceptron

### Variant of the Perceptron Algorithm
Let $w(t)$ be the weight vector estimate and $x_{(t)}$ the corresponding feature vector presented at the $t^{th}$ iteration.

The algorithm is as follows:
* $w(t+1) = w(t) + \rho x_{(t)}$ if $x_{(t)} \in \omega_1$ and $w^T(t)x_{(t)} \le 0$
* $w(t+1) = w(t) - \rho x_{(t)}$ if $x_{(t)} \in \omega_2$ and $w^T(t)x_{(t)} \ge 0$
* $w(t+1) = w(t)$ otherwise

* if current training example is classified correctly, no action is taken
* if sample is misclassified, the weight vector is corrected by adding (subtracting) an amount proportional to $x_{(t)}$

---
**Navigation**
[[L6A-Slide-15|Previous ← Perceptron Convergence Proof (conclusion)]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-17|Next → The Perceptron Network]]