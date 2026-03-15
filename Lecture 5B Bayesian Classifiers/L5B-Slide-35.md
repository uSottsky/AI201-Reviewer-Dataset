# Maximum Likelihood Estimation (MLE)

Choose the parameter that maximizes the probability of observed data $P(X;\theta)$.

Let $x_{1},x_{2},...,x_{N}$ be random samples drawn from a distribution with pdf $p(x;\theta)$ and unknown parameter vector $\theta$. Form joint pdf $p(X;\theta)$ where $X=\{x_{1},x_{2},...,x_{N}\}$ is the set of samples.

For statistically independent samples we have the likelihood function of $\theta$ with respect to $X$:
$$p(X;\theta) \equiv p(x_{1},x_{2},...,x_{N};\theta) = \prod_{k=1}^{N}p(x_{k};\theta)$$

The Maximum Likelihood Estimation (MLE) method estimates $\theta$ so that the likelihood function is maximized:
$$\hat{\theta}_{MLE} = \arg \max_{\theta}\prod_{k=1}^{N}p(x_{k};\theta)$$

Define the log likelihood function as $L(\theta) = \ln\prod_{k=1}^{N}p(x_{k};\theta)$. Maximum likelihood estimate $\hat{\theta}_{MLE}$ is computed by maximizing $L(\theta)$ which is equivalent to solving:
$$\frac{\partial L(\theta)}{\partial\theta} = \sum_{k=1}^{N}\frac{\partial \ln p(x_{k};\theta)}{\partial\theta} = \sum_{k=1}^{N}\frac{1}{p(x_{k};\theta)}\frac{\partial p(x_{k};\theta)}{\partial\theta} = 0$$

---
**Navigation**
[[L5B-Slide-34|Previous ← Estimation of Unknown Probability Density Functions]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-36|Next → Properties of MLE]]