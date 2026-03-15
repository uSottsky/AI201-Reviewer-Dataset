# Nondiagonal Covariance Matrix

The hyperplane between two classes is defined as:
$$g_{i}(x) - g_{j}(x) = 0$$

Expanding the discriminant functions:
$$\mu_{i}^{T}\Sigma^{-1}x + \ln P(\omega_{i}) - \frac{1}{2}\mu_{i}^{T}\Sigma^{-1}\mu_{i} - \mu_{j}^{T}\Sigma^{-1}x - \ln P(\omega_{j}) + \frac{1}{2}\mu_{j}^{T}\Sigma^{-1}\mu_{j} = 0$$

Rearranging and combining terms:
$$(\mu_{i}-\mu_{j})^{T}\Sigma^{-1}x - \frac{1}{2}(\mu_{i}-\mu_{j})^{T}\Sigma^{-1}(\mu_{i}+\mu_{j}) + \ln\left(\frac{P(\omega_{i})}{P(\omega_{j})}\right) = 0$$

Factoring out the components to match the form $w^{T}(x - x_0) = 0$:
$$\underbrace{(\mu_{i}-\mu_{j})^{T}\Sigma^{-1}}_{w^{T}} \left( x - \underbrace{\left[ \frac{1}{2}(\mu_{i}+\mu_{j}) - \ln\left(\frac{P(\omega_{i})}{P(\omega_{j})}\right) \frac{\mu_{i}-\mu_{j}}{(\mu_{i}-\mu_{j})^{T}\Sigma^{-1}(\mu_{i}-\mu_{j})} \right]}_{x_0} \right) = 0$$

Hyperplanes: $g_{ij}(x) = w^{T}(x-x_{0}) = 0$ where:
* $w = \Sigma^{-1}(\mu_{i}-\mu_{j})$
* $x_{0} = \frac{1}{2}(\mu_{i}+\mu_{j}) - \ln\left(\frac{P(\omega_{i})}{P(\omega_{j})}\right)\frac{\mu_{i}-\mu_{j}}{(\mu_{i}-\mu_{j})^{T}\Sigma^{-1}(\mu_{i}-\mu_{j})}$

The decision hyperplane is no longer orthogonal to the vector $\mu_{i}-\mu_{j}$ but to the linear transformation $\Sigma^{-1}(\mu_{i}-\mu_{j})$. All other comments for the diagonal covariance matrix still applicable.

---
**Navigation**
[[L5B-Slide-28|Previous ← Compact vs Noncompact Classes]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-30|Next → Equal Covariance Matrices]]