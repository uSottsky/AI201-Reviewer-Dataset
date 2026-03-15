# Optimization Review

### Quadratic Cost functions
Let $J(\theta)$ assume the quadratic form:
$$J(\theta) = b - p^T\theta + \frac{1}{2}\theta^T R\theta$$
where $R$ is positive definite. Then
$$\frac{\partial J(\theta)}{\partial\theta} = R\theta - p$$

Thus the optimum value is:
$$R\theta^0 = p$$

**Theorem:**
A cost function of the quadratic form (where $R$ is positive definite) converges to its optimal value if:
$$\mu < \frac{2}{\lambda_{max}}$$
where $\lambda_{max}$ is the maximum eigenvalue of $R$.

---
**Navigation**
[[L6A-Slide-04|Previous ← Gradient Descent Convergence]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-06|Next → Nonquadratic Cost Functions]]