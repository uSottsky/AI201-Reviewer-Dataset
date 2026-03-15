# The Gaussian PDF (Univariate)

> ![[Pasted image 20260315202429.png]]
> Reference: Slide 16 - Two 1D Gaussian curves (a) centered at 0 with wider variance, (b) centered at 1 with narrower variance.

**Univariate Gaussian:**
$$p(x) = \frac{1}{\sqrt{2\pi}\sigma}\exp\left(-\frac{(x-\mu)^{2}}{2\sigma^{2}}\right), \quad x\in R$$

where:
* $\mu = E[x] \equiv \int_{-\infty}^{+\infty}xp(x)dx$
* $\sigma^{2} = E[(x-\mu)^{2}] = \int_{-\infty}^{+\infty}(x-\mu)^{2}p(x)dx$

---
**Navigation**
[[L5B-Slide-15|Previous ← Discriminant Functions and Decision Surfaces]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-17|Next → The Gaussian PDF (Multivariate)]]