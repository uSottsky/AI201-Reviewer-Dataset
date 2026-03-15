# Optimization Review

### Nonquadratic Cost Functions
If $J(\theta)$ is not quadratic, we invoke Taylor's theorem and assume that at some step near a stationary point, $\theta^0$, the cost function can be approximated as:
$$J(\theta) = J(\theta^0) + (\theta - \theta^0)^T g + \frac{1}{2}(\theta - \theta^0)^T H (\theta - \theta^0)$$

where:
#### $$g = \frac{\partial J(\theta)}{\partial\theta} \bigg|_{\theta=\theta^0} , \quad H(i,j) = \frac{\partial^2 J(\theta)}{\partial\theta_i \partial\theta_j} \bigg|_{\theta=\theta^0}$$

In the neighborhood of $\theta^0$ the cost function is given approximately by a quadratic form and the convergence of the algorithm is controlled by the eigenvalues of the Hessian matrix.

---
**Navigation**
[[L6A-Slide-05|Previous ← Quadratic Cost Functions]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-07|Next → Linear Classifiers]]