# Maximum A Posteriori (MAP) Estimation

Choose the parameter that is most probable given the observed data and prior belief.

In MAP estimation we consider $\theta$ as a random variable and estimate it conditioned on the occurrence of samples $x_{1},x_{2},...,x_{N}$.
Let $X=\{x_{1},x_{2},...,x_{N}\}$, $x_{i}\in R^{l}$. Bayes theorem:
$$p(\theta|X) = \frac{p(\theta)p(X|\theta)}{p(X)}$$

The MAP estimate $\hat{\theta}_{MAP}$ is defined at the point where $p(\theta|X)$ becomes maximum, i.e., when:
$$\frac{\partial}{\partial\theta}p(\theta|X) = \frac{\partial}{\partial\theta}p(\theta)p(X|\theta) = 0$$

The prior probability is not involved since it is independent of $\theta$.

**MAP estimate:**
$$\hat{\theta}_{MAP} = \arg \max_{\theta}\prod_{k=1}^{N}p(\theta)p(x_{k}|\theta)$$

---
**Navigation**
[[L5B-Slide-36|Previous ← Properties of MLE]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-38|Next → The Naive Bayes Classifier]]