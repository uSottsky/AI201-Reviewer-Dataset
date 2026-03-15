# Equiprobable Classes

![[Pasted image 20260315184707.png]]

For single feature ($l=1$), threshold at $x_0$ divides feature space into 2 regions $R_1$ and $R_2$.

**Classification rule:**
- $x < x_0$: classify $x$ as $\omega_1$
- $x > x_0$: classify $x$ as $\omega_2$

Overlapping portions of $p(x|\omega_1)$ and $p(x|\omega_2)$ lead to errors.

$$
P_{\text{error}} = P_e = \frac{1}{2} \int_{-\infty}^{x_0} p(x|\omega_2)dx + \frac{1}{2} \int_{x_0}^{\infty} p(x|\omega_1)dx
$$

Bayes Classification Rule gives us the most probable classification.

 
---

10/44

[[L5B-Slide-09|Previous ← Bayes Classification Rule]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-11|Next → Bayes Classifier is Optimal]]