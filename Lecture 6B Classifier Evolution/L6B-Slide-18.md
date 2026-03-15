# Pearson Correlation Coefficient

$$r = \frac{1}{N} \sum_{i=1}^N \frac{(\hat{y}_i - \hat{m})(y_i - m)}{s\hat{s}}$$

where $m = (1/N)\sum_{i=1}^N y_i$ is the mean of the target, $\hat{m} = (1/N)\sum_{i=1}^N \hat{y}_i$ is the mean of the predictions, and $s = \sqrt{(1/N)\sum_{i=1}^N (y_i - m)^2}$, $\hat{s} = \sqrt{(1/N)\sum_{i=1}^N (\hat{y}_i - \hat{m})^2}$ are the corresponding standard deviations.

* $-1 < r < 1$
* $r$ near or below zero: useless predictor
* $r$ near $1$: very good predictor

**Coefficient of Determination aka Normalized MSE**
$$Q^2 = 1 - \frac{\sum_{i=1}^N (y_i - \hat{y}_i)^2}{\sum_{i=1}^N (y_i - m)^2}$$

---
**Navigation**
[[L6B-Slide-17|Previous ← MSE and MAE]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-19|Next → References]]