# Decision Hyperplanes

**Recall:**
$$g_{i}(x) = -\frac{1}{2}x^{T}\Sigma_{i}^{-1}x + \frac{1}{2}x^{T}\Sigma_{i}^{-1}\mu_{i} - \frac{1}{2}\mu_{i}^{T}\Sigma_{i}^{-1}\mu_{i} + \frac{1}{2}\mu_{i}^{T}\Sigma_{i}^{-1}x + \ln P(\omega_{i}) + c_{i}$$
* quadratic contribution: $x^{T}\Sigma_{i}^{-1}x$

**Assume covariance matrix is the same for all classes** (i.e., $\Sigma_{i}=\Sigma$).
Quadratic term and the constants $c_{i}$ will be the same in all discriminant functions and will not matter in the computation for the maximum.

Redefine $g_{i}(x)$ as:
$$g_{i}(x) = w_{i}^{T}x + w_{i0}$$
where:
* $w_{i} = \Sigma^{-1}\mu_{i}$
* $w_{i0} = \ln P(\omega_{i}) - \frac{1}{2}\mu_{i}^{T}\Sigma^{-1}\mu_{i}$

The decision surfaces are hyperplanes since $g_{i}(x)$ is a linear function of $x$.

---
**Navigation**
[[L5B-Slide-24|Previous ← Decision Curve: Hyperbola Visualization]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-26|Next → Diagonal Covariance Matrix with Equal Elements]]