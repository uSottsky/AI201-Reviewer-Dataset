# Discriminant Functions and Decision Surfaces

**Decision Surface**
* decision surface separates contiguous regions $R_{i}$ and $R_{j}$
* minimum error probability: decision surface is $P(\omega_{i}|x) - P(\omega_{j}|x) = 0$
* difference is positive/negative for one side/other side of decision surface

Define the **discriminant function** as $g_{i}(x) \equiv f(P(\omega_{i}|x))$ where $f(\cdot)$ is a monotonically increasing function.

Decision test can be equivalently stated as:
* classify $x$ in $\omega_{i}$ if $g_{i}(x) > g_{j}(x)$ $\forall j\ne i$

**Decision surface:**
* $g_{ij}(x) \equiv g_{i}(x) - g_{j}(x) = 0 \quad i,j=1,2,...,M, \quad i\ne j$

Classification problem has been recast as one of minimizing classification error probability or risk.
* problems with complicated pdfs: preferable to compute decision surfaces directly by means of alternative costs
* discriminant functions and surfaces may or may not have any relation to Bayesian classification and are in general suboptimal with respect to Bayesian classifiers.

---
**Navigation**
[[L5B-Slide-14|Previous ← Risk Minimization: Two-Class Case]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-16|Next → The Gaussian PDF (Univariate)]]