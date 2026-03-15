# Logistic Discrimination

### Logistic Discrimination and LDA
Under the Gaussian assumption and for equal variance matrices $(\Sigma_1 = \Sigma_2 = \Sigma)$ across all classes, the following holds:
$$\ln \frac{P(\omega_1|x)}{P(\omega_2|x)} = \underbrace{\frac{1}{2}(\mu_2^T \Sigma^{-1} \mu_2 - \mu_1^T \Sigma^{-1} \mu_1)}_{w_0} + \underbrace{(\mu_1 - \mu_2)^T \Sigma^{-1}}_{w^T} x = w_0 + w^T x$$

However, LDA is not identical to logistic discrimination.
* **LDA:** class probability densities are assumed to be Gaussian and the unknown parameters are estimated by maximizing Eqn 10 directly. The marginal densities $p(x_k)$ enter implicitly into this equation.
* **Logistic Discrimination:** marginal densities contribute to $C$ and do not affect the solution.

If the Gaussian assumption is a reasonable one for the problem at hand, LDA is the natural approach, otherwise Logistic Discrimination is a better candidate since it relies on fewer assumptions.

In practice, there is little difference between the results obtained by the two methods.

---
**Navigation**
[[L6A-Slide-30|Previous ← Logistic Discrimination Likelihood]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-32|Next → References]]