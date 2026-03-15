# Logistic Regression (Parametric Model)


Let $p(y|x,w) = Ber(y|\mu(x))$ where $\mu(x) = \mathbb{E}[y|x] = p(y=1|x)$ and has the form:

$$\mu(x) = sigmoid(w^{T}x)$$

The sigmoid (or logistic or logit) function is defined as:
$$sigmoid(\eta) = \frac{1}{1+\exp(-\eta)} = \frac{e^{\eta}}{e^{\eta}+1}$$

* squashing function that maps the real number line to $[0, 1]$ so that output can be interpreted as a probability.

![[Pasted image 20260315164843.png]]
> Reference: Slide 15 - Graph of the Sigmoid (logistic) curve ranging from 0 to 1 on the y-axis, forming an S-shape.



15/25

---
**Navigation**
[[L5A-Slide-14|Previous ← Bernoulli Distribution]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-16|Next → Logistic Regression Equation]]