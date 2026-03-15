# Bias-Variance Dilemma


If a model has many parameters involved with respect to $N$, it will fit the idiosyncrasies of the specific data set resulting in low bias but will yield high variance as we change from one dataset to another.

![[Pasted image 20260315215742.png]]
> Reference: Slide 28 - Graph illustrating the Bias-Variance Dilemma. It shows a smooth true function $f(x)$, a high bias/low variance linear fit $g(x)$, and an overfitted, low bias/high variance polynomial fit $g_1(x)$ that perfectly hits all training points but oscillates wildly in between.


On the other extreme, if we choose a model that does not depend on $\mathcal{D}$, the variance is zero but the bias will be large.

---
**Navigation**
[[L6A-Slide-27|Previous ← Bias-Variance Dilemma]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-29|Next → Logistic Discrimination]]