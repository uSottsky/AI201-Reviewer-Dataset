# Perceptron

Similarly, let:
$$\gamma = \max_{\tilde{Y} \subseteq \omega_1 \cup \omega_2} \sum_{x \in \tilde{Y}} \delta_x w^{*T} x$$

Recall that the summation in this equation is negative, therefore its maximum value over all possible subsets of $x$'s will also be a negative number.
Thus:
$$||w(t+1) - \alpha w^*||^2 \le ||w(t) - \alpha w^*||^2 + \rho_t^2 \beta^2 - 2\rho_t \alpha |\gamma|$$

Choose:
$$\alpha = \frac{\beta^2}{2|\gamma|}$$

and apply the above equation successively for steps $t, t-1,...,0$. Then:
$$||w(t+1) - \alpha w^*||^2 \le ||w(0) - \alpha w^*||^2 + \beta^2 \left( \sum_{k=0}^t \rho_k^2 - \sum_{k=0}^t \rho_k \right)$$

If the sequence $\rho_t$ is chosen to satisfy the following conditions:
$$\lim_{t \rightarrow \infty} \sum_{k=0}^t \rho_k = \infty \quad \text{(2)}$$
$$\lim_{t \rightarrow \infty} \sum_{k=0}^t \rho_k^2 < \infty \quad \text{(3)}$$

then there will be a constant $t_0$ such that the right-hand side of Eqn 1 becomes nonpositive.

---
**Navigation**
[[L6A-Slide-13|Previous ← Perceptron Convergence Theorem]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-15|Next → Perceptron Convergence Proof (conclusion)]]