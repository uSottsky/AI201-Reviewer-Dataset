# Perceptron

Therefore:
$$0 \le ||w(t_0+1) - \alpha w^*|| \le 0$$
or
$$w(t_0+1) = \alpha w^*$$
that is, the Perceptron Algorithm converges to a solution in a finite number of steps.

**Value of $\rho_t$ (e.g. $\rho_t = c/t$):**
* $\rho_t$ should vanish as $t \rightarrow \infty$ (cf. Eqn 3)
* $\rho_t$ should not go to zero very fast (cf. Eqn 2)

Under certain conditions, a constant learning rate $(\rho_t = \rho)$ works.

---
**Navigation**
[[L6A-Slide-14|Previous ← Perceptron Convergence Proof (cont.)]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-16|Next → Variant of the Perceptron Algorithm]]