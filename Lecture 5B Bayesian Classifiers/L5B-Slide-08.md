# Bayes Decision Theory

Consider two classes $\omega_1, \omega_2$. Assume that the a priori probabilities $P(\omega_1), P(\omega_2)$ are known.

- if $P(\omega_1), P(\omega_2)$ are not known, compute them from training data:  
  Let $N$ be the total number of patterns and $N_1, N_2$ of them belong to class $\omega_1, \omega_2$ respectively. Then $P(\omega_1) = N_1/N$ and $P(\omega_2) = N_2/N$

Let the class conditional probability density function $p(x|\omega_i), i = 1, 2$ describe the distribution of the feature vectors of each class.

**Bayes Theorem:**

![[Pasted image 20260315201556.png]]

**Bayes Classification Rule:**

- $P(\omega_1|x) > P(\omega_2|x)$: classify $x$ as $\omega_1$  
- $P(\omega_1|x) < P(\omega_2|x)$: classify $x$ as $\omega_2$  
- (in case of equality, $x$ can be classified as $\omega_1$ or $\omega_2$)
---

8/44

[[L5B-Slide-07|Previous ← Classification System]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-09|Next → Bayes Classification Rule]]