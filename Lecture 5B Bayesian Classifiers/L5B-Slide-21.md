# The Bayesian Classifier for Normally Distributed Classes

Consider the Bayesian classifier for the multi class case where the pdfs $p(x|\omega_{i})$ describing the data distribution are normal distributions.

Define the following discriminant functions:
$$g_{i}(x) = \ln(p(x|\omega_{i})P(\omega_{i})) = \ln p(x|\omega_{i}) + \ln P(\omega_{i})$$
$$= -\frac{1}{2}(x-\mu_{i})^{T}\Sigma_{i}^{-1}(x-\mu_{i}) + \ln P(\omega_{i}) + c_{i}$$
$$= -\frac{1}{2}x^{T}\Sigma_{i}^{-1}x + \frac{1}{2}x^{T}\Sigma_{i}^{-1}\mu_{i} - \frac{1}{2}\mu_{i}^{T}\Sigma_{i}^{-1}\mu_{i} + \frac{1}{2}\mu_{i}^{T}\Sigma_{i}^{-1}x + \ln P(\omega_{i}) + c_{i}$$
where $c_{i} = -(l/2)\ln 2\pi - (1/2)\ln|\Sigma_{i}|$

For the 2-dimensional case where $\Sigma_{i} = \begin{bmatrix} \sigma_{i}^{2} & 0 \\ 0 & \sigma_{i}^{2} \end{bmatrix}$ :
$$g_{i}(x) = -\frac{1}{2\sigma_{i}^{2}}(x_{1}^{2}+x_{2}^{2}) + \frac{1}{\sigma_{i}^{2}}(\mu_{i1}x_{1}+\mu_{i2}x_{2}) - \frac{1}{2\sigma_{i}^{2}}(\mu_{i1}^{2}+\mu_{i2}^{2}) + \ln P(\omega_{i}) + c_{i}$$

The decision curves $g_{i}(x) - g_{j}(x) = 0$ are quadrics (ellipsoids, parabolas, hyperbolas, pairs of lines).
* The Bayesian classifier is a quadratic classifier that partitions the feature space through quadric decision surfaces.
* For higher dimensional feature spaces, the decision surfaces are hyperquadrics.

---
**Navigation**
[[L5B-Slide-20|Previous ← Isocurves: Nondiagonal Covariance]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-22|Next → Decision Curves (Ellipses and Hyperbolas)]]