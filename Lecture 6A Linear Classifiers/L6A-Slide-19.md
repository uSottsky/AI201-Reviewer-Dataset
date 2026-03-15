# Mean Square Error Estimation

### Least Squares Method
Given a vector $x$, the output of the classifier will be $w^T x$ (thresholds are accommodated by vector extension).

Denote desired vector output as $y(x) \equiv y = \pm 1$. Compute weight vector that minimizes the mean square error (MSE) between the desired and true outputs, i.e.,
$$J(w) = E[|y - x^T w|^2]$$
so that
$$\hat{w} = \arg \min_w J(w)$$

Cost function $J(w)$ is:
$$J(w) = P(\omega_1)\int(1 - x^T w)^2 p(x|\omega_1)dx + P(\omega_2)\int(1 + x^T w)^2 p(x|\omega_2)dx$$

* class $\omega_1$ error: $1 - x^T w$
* class $\omega_2$ error: $-1 - x^T w = -(1 + x^T w)$

---
**Navigation**
[[L6A-Slide-18|Previous ← The Pocket Algorithm]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-20|Next → Minimizing J(w)]]