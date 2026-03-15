# Spam Filter: Classification Calculation

**Priors:** $P(\omega=H)=\frac{6}{11}$ and $P(\omega=S)=\frac{5}{11}$

**Likelihood (Ham):**                                                           **Likelihood (Spam):**
* $P(x_{1}=1|\omega=H)=3/6$                                                  $P(x_{1}=1|\omega=S)=1/5$
* $P(x_{2}=1|\omega=H)=1/6$                                                  $P(x_{2}=1|\omega=S)=3/5$
* $P(x_{3}=1|\omega=H)=2/6$                                                  $P(x_{3}=1|\omega=S)=3/5$
* $P(x_{4}=1|\omega=H)=3/6$                                                  $P(x_{4}=1|\omega=S)=1/5$
* $P(x_{5}=1|\omega=H)=3/6$                                                  $P(x_{5}=1|\omega=S)=1/5$
* $P(x_{6}=1|\omega=H)=4/6$                                                  $P(x_{6}=1|\omega=S)=1/5$
* $P(x_{7}=1|\omega=H)=4/6$                                                  $P(x_{7}=1|\omega=S)=3/5$
* $P(x_{8}=1|\omega=H)=4/6$                                                  $P(x_{8}=1|\omega=S)=1/5$


**Class of $D_{A}=[1~0~0~1~1~0~1]^{T}$?**
Recall:
$$P(\omega|x_{1},x_{2},...,x_{d}) = \frac{\prod_{i=1}^{d}P(x_{i}|\omega)P(\omega)}{\sum_{\omega}\prod_{i=1}^{d}P(x_{i}|\omega)P(\omega)}$$

#### $$P(H|[1~0~0~1~1~0~1]^{T}) = \frac{\left(\frac{5}{6}\cdot\frac{2}{3}\cdot\frac{2}{2}\cdot\frac{3}{3}\right)\frac{6}{11}}{\left(\frac{5}{6}\cdot\frac{2}{3}\cdot\frac{2}{2}\cdot\frac{3}{3}\right)\frac{6}{11} + \left(\frac{1}{5}\cdot\frac{2}{5}\cdot\frac{2}{5}\cdot\frac{1}{5}\right)\frac{5}{11}} = 0.9988$$

---
**Navigation**
[[L5B-Slide-41|Previous ← Spam Filter: Training Set Example]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-43|Next → Spam Filter: Laplace and Lambda Smoothing]]