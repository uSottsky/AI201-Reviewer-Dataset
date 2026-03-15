# Optimality of Bayesian Classifier

We show that the Bayes Classifier is optimal with respect to minimizing classification errors.

**Proof:**
Error occurs when $x\in R_{2}$ although it belongs to $\omega_{1}$ or when $x\in R_{1}$ although it belongs to $\omega_{2}$.
Probability of error: $P_{e}=P(x\in R_{2},\omega_{1})+P(x\in R_{1},\omega_{2})$ where $P(\cdot,\cdot)$ is the joint probability.

$$P_{e} = P(x\in R_{2}|\omega_{1})P(\omega_{1}) + P(x\in R_{1}|\omega_{2})P(\omega_{2})$$
$$= P(\omega_{1})\int_{R_{2}}p(x|\omega_{1})dx + P(\omega_{2})\int_{R_{1}}p(x|\omega_{2})dx$$
$$= \int_{R_{2}}P(\omega_{1}|x)p(x)dx + \int_{R_{1}}P(\omega_{2}|x)p(x)dx \quad \text{(by Bayes Rule)}$$

For minimum error we partition $R_{1}$ and $R_{2}$ so that:
* $R_{1}: P(\omega_{1}|x) > P(\omega_{2}|x)$
* $R_{2}: P(\omega_{2}|x) > P(\omega_{1}|x)$

Since $R_{1}\cup R_{2}$ covers all space, $P(\omega_{1}) = \int_{R_{1}}P(\omega_{1}|x)p(x)dx + \int_{R_{2}}P(\omega_{1}|x)p(x)dx$. Combining this, we obtain:
$$P_{e} = P(\omega_{1}) - \int_{R_{1}}(P(\omega_{1}|x) - P(\omega_{2}|x))p(x)dx$$

Thus, the probability of error is minimized if $R_{1}$ is the region of space in which $P(\omega_{1}|x) > P(\omega_{2}|x)$.

---
**Navigation**
[[L5B-Slide-10|Previous ← Equiprobable Classes]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-12|Next → M Class Bayesian Classifier]]