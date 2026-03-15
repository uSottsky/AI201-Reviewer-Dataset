# Perceptron

### Perceptron Convergence Theorem

**Theorem:**
The Perceptron Algorithm converges to a solution in a finite number of steps provided that the sequence $\rho_t$ is properly chosen.
Solution is not unique since there are an infinite number of hyperplanes that can separate the two linearly separable classes.

**Proof:**
Let $\alpha$ be a positive real number and $w^*$ a solution. Then:
$$w(t+1) - \alpha w^* = w(t) - \alpha w^* - \rho_t \sum_{x \in Y} \delta_x x$$

Square the Euclidean norm of both sides:
$$||w(t+1) - \alpha w^*||^2 = ||w(t) - \alpha w^*||^2 + \rho_t^2 \bigg|\bigg|\sum_{x \in Y} \delta_x x\bigg|\bigg|^2 - 2\rho_t \sum_{x \in Y} \delta_x (w(t) - \alpha w^*)^T x$$

Since $\sum_{x \in Y} \delta_x w^T(t) x < 0$, we have:
$$||w(t+1) - \alpha w^*||^2 \le ||w(t) - \alpha w^*||^2 + \rho_t^2 \bigg|\bigg|\sum_{x \in Y} \delta_x x\bigg|\bigg|^2 + 2\rho_t \alpha \sum_{x \in Y} \delta_x w^{*T} x$$

Define $\beta^2 = \max_{\tilde{Y} \subseteq \omega_1 \cup \omega_2} ||\sum_{x \in \tilde{Y}} \delta_x x||^2$, i.e., it is the maximum value that the vector norm can take by considering all possible subsets of the available training feature vectors.

---
**Navigation**
[[L6A-Slide-12|Previous ← Geometric Interpretation]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-14|Next → Perceptron Convergence Proof (cont.)]]