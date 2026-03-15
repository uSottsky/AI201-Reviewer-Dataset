# LMS Algorithm

### Stochastic Approximation
To solve Eqn 5, the computation of the correlation matrix and cross-correlation vector is required, presupposing knowledge of the underlying distributions which in general is not known. We attempt to solve Eqn 4 without this information.

Consider the equation $E[F(x_k, w)] = 0$, where $x_k, k=1,2,...$ is a sequence of random vectors from the same distribution.
Let $F(\cdot, \cdot)$ be a function and $w$ the vector of the unknown parameters. Adopt the iterative scheme:
$$\hat{w}(k) = \hat{w}(k-1) + \rho_k F(x_k, \hat{w}(k-1))$$

The mean value (which cannot be computed due to lack of information) is replaced by samples of the random variables resulting from the experiments.
This iterative scheme converges in probability to the solution $w$ of the original equation provided that the sequence satisfies the following conditions:
$\sum_{k=1}^\infty \rho_k \rightarrow \infty$, $\sum_{k=1}^\infty \rho_k^2 < \infty$, and $\rho_k \rightarrow 0$.

Consider the equation $E[x_k - w] = 0$. For $\rho_k = \frac{1}{k}$ the iteration becomes:
$$\hat{w}(k) = \hat{w}(k-1) + \frac{1}{k}[x_k - \hat{w}(k-1)] = \frac{k-1}{k}\hat{w}(k-1) + \frac{1}{k}x_k$$

For large values of $k$:
$$\hat{w}(k) = \frac{1}{k}\sum_{r=1}^k x_r \quad \text{(6)}$$
that is, the solution is the sample mean of the measurements.

---
**Navigation**
[[L6A-Slide-22|Previous ← Multiclass Case]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-24|Next → The LMS (Widrow-Hoff) Algorithm]]