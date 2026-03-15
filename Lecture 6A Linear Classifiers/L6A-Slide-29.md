# Logistic Discrimination

In logistic discrimination the logarithm of the likelihood ratio is modeled via linear functions, i.e.,
$$\ln \frac{P(\omega_i|x)}{P(\omega_M|x)} = w_{i,0} + w_i^T x, \quad i=1,2,...,M-1$$

Any class other than $\omega_M$ can be used in the denominator. The unknown parameters $w_{i,0}, w_i, i=1,2,...,M-1$ must be chosen to ensure that probabilities add to one, i.e., $\sum_{i=1}^M P(\omega_i|x) = 1$.
Thus the a posteriori probabilities are:
$$P(\omega_M|x) = \frac{1}{1 + \sum_{i=1}^{M-1} \exp(w_{i,0} + w_i^T x)}$$
$$P(\omega_i|x) = \frac{\exp(w_{i,0} + w_i^T x)}{1 + \sum_{i=1}^{M-1} \exp(w_{i,0} + w_i^T x)}$$

For two classes these equations simplify to:
$$P(\omega_2|x) = \frac{1}{1 + \exp(w_{1,0} + w_1^T x)}$$
$$P(\omega_1|x) = \frac{\exp(w_{1,0} + w_1^T x)}{1 + \exp(w_{1,0} + w_1^T x)}$$

The unknown parameters are estimated using maximum likelihood estimation.

---
**Navigation**
[[L6A-Slide-28|Previous ← Bias-Variance Dilemma Graph]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-30|Next → Logistic Discrimination Likelihood]]