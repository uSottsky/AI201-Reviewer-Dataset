# Discriminant Functions and Decision Surfaces

**Decision Surface** separates contiguous regions $R_i$ and $R_j$.  
Minimum-error decision surface: $P(\omega_i|x) - P(\omega_j|x) = 0$.

Define the **discriminant function**  
$g_i(x) \equiv f(P(\omega_i|x))$ where $f(\cdot)$ is monotonically increasing.

**Classification rule:**  
classify $x$ in $\omega_i$ if $g_i(x) > g_j(x)$ for all $j \neq i$.

**Decision surface:**  
$g_{ij}(x) \equiv g_i(x) - g_j(x) = 0$

- Problems with complicated pdfs → compute decision surfaces directly  
- Discriminant functions may be suboptimal compared to true Bayesian classifiers

An image is needed here.

15/44

[[L5B-Slide-14|Previous ← Two-Class Case]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-16|Next → Bayesian Classification for Normal Distribution (Univariate)]]