# Mean Square Error Regression

Let $y, x$ be two random variables where $y \in \mathbb{R}^{M \times 1}$ and $x \in \mathbb{R}^{l \times 1}$. Assume that they are described by joint pdf $p(y,x)$.

Estimate $y$ given $x$ that is obtained from an experiment. This framework encompasses the classification task.
* For example, given a feature vector $x$, estimate the value of the class label $y$ which is $\pm 1$ for the 2 class case.

For the more general framework, values of $y$ may not be discrete. For $y \in \mathbb{R}$,
$$y = f(x) + \epsilon$$
where $f(\cdot)$ is unknown and $\epsilon$ is a noise source. Predict the value of $y$ given the value of $x$.

**Regression task:** design a function $g(x)$ based on a set of training data points $(y_i, x_i), i=1,2,...,N$ so that the predicted value $\hat{y} = g(x)$.

Commonly used optimality criterion for regression is MSE.
The mean square estimate $\hat{y}$ of the random vector $y$ given the value of $x$ is defined as:
$$\hat{y} = \arg \min_{\tilde{y}} E[||y - \tilde{y}||^2]$$

The mean value above is with respect to the conditional pdf $p(y|x)$.
It can be shown that the optimal estimate is the mean value of $y$, i.e.,
$$\hat{y} = E[y|x] \equiv \int_{-\infty}^{\infty} y p(y|x)dy.$$

---
**Navigation**
[[L6A-Slide-25|Previous ← Sum of Error Squares Estimation]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-27|Next → Bias-Variance Dilemma]]