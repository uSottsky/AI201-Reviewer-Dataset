# Bias-Variance Dilemma

A regressor or classifier can be viewed as learning machines realizing a function or a set of functions $g(x)$ that attempt to estimate the corresponding value or class label $y$ and make a decision based on these estimates.

The functions $g(\cdot)$ are estimated using a finite training data set $\mathcal{D} = \{(y_i, x_i)\}, i=1,2,...,N$ and a suitable methodology (e.g., mean square error, sum of error squares, LMS).

We examine the capabilities of $g(x; \mathcal{D})$ to approximate the MSE optimal regressor $E[y|x]$ and how this is affected by finite size, $N$, of the training data set.
* The approximation may be very good for a specific training data set $\mathcal{D}$ but very bad for another.

The effectiveness of an estimator can be evaluated by computing its mean square deviation from the desired optimal value.
This is achieved by averaging over all possible sets $\mathcal{D}$ of size $N$, i.e., $E_\mathcal{D}[(g(x; \mathcal{D}) - E[y|x])^2]$.

Expanding this yields:
$$E_\mathcal{D}[(g(x; \mathcal{D}) - E[y|x])^2] = \underbrace{(E_\mathcal{D}[g(x; \mathcal{D})] - E[y|x])^2}_{\text{bias}^2} + \underbrace{E_\mathcal{D}[(g(x; \mathcal{D}) - E_\mathcal{D}[g(x; \mathcal{D})])^2]}_{\text{variance}}$$

* **Bias:** measures the extent to which the average (over all data sets) of the model function $g(x; \mathcal{D})$ differs from the desired function $E[y|x]$.
* **Variance:** measures the extent to which the function $g(x; \mathcal{D})$ is sensitive to the particular choice of data set.

---
**Navigation**
[[L6A-Slide-26|Previous ← Mean Square Error Regression]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-28|Next → Bias-Variance Dilemma Graph]]