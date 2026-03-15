# Properties of MLE

**1. Unbiased estimate:** mean is the true value of the unknown parameter. 

**MLE is asymptotically unbiased:**
$$\lim_{N\rightarrow\infty}E[\hat{\theta}_{MLE}]=\theta_{0}$$
(estimate converges in the mean to the true value)

**2. MLE is asymptotically consistent (weak version):**
$$\lim_{N\rightarrow\infty}Pr\{||\hat{\theta}_{MLE}-\theta_{0}||\le\epsilon\}=1 \quad \text{for arbitrarily small } \epsilon$$
(estimate converges in probability)

**3. MLE is asymptotically consistent (strong version):**
$$\lim_{N\rightarrow\infty}E[||\hat{\theta}_{MLE}-\theta_{0}||^{2}]=0$$
(estimate converges in the mean square, i.e., for large N, variance of the estimate tends to zero)

**4. MLE is asymptotically efficient:** (achieves the lowest value of variance that any estimate can achieve (Cramer-Rao lower bound))

**5. The pdf of the MLE as $N\rightarrow\infty$ approaches the Gaussian distribution with mean $\theta_{0}$**

**6. MLE is invariant under reparameterization:** $g(\theta_{MLE})$ is a MLE for $g(\theta)$

---
**Navigation**
[[L5B-Slide-35|Previous ← Maximum Likelihood Estimation (MLE)]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-37|Next → Maximum A Posteriori (MAP) Estimation]]