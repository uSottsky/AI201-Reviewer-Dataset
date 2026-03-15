# The Gaussian PDF (Multivariate)

**Multivariate Gaussian:**
$$p(x) = \frac{1}{(2\pi)^{l/2}|\Sigma|^{1/2}}\exp\left(-\frac{1}{2}(x-\mu)^{T}\Sigma^{-1}(x-\mu)\right), \quad x\in R^{l}$$

where
* $\mu = E[x] \in R^{l}$
* $\Sigma = E[(x-\mu)(x-\mu)^{T}] \in R^{l}\times R^{l}$

For the 2-dimensional Gaussian:
$$
\Sigma = E \left[ \begin{bmatrix} x_1 - \mu_1 \\ x_2 - \mu_2 \end{bmatrix} [x_1 - \mu_1, x_2 - \mu_2] \right] = \begin{bmatrix} \sigma_{1}^{2} & \sigma_{12} \\ \sigma_{21} & \sigma_{2}^{2} \end{bmatrix}
$$

---
**Navigation**
[[L5B-Slide-16|Previous ← The Gaussian PDF (Univariate)]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-18|Next → Isocurves: Spherically Symmetric]]