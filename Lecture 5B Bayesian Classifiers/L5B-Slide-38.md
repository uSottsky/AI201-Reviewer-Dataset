# The Naive Bayes Classifier

Assume that the individual features $x_j$ ($j = 1, 2, ..., l$) are statistically independent. Thus,
$$p(x|\omega_{i}) = \prod_{j=1}^{l}p(x_{j}|\omega_{i})$$

To estimate $l$ one-dimensional pdfs for each of the classes, $lN$ datapoints are enough to obtain good estimates instead of $N^{l}$ points.

The Naive Bayes Classifier assigns an unknown sample $x=[x_{1},x_{2},...,x_{l}]^{T}$ to the class:
$$\omega_{NB} = \arg \max_{\omega_{i}}\prod_{j=1}^{l}p(x_{j}|\omega_{i})$$

The Naive Bayes classifier is known to perform very well for many real world datasets even when the independence assumption is violated.

---
**Navigation**
[[L5B-Slide-37|Previous ← Maximum A Posteriori (MAP) Estimation]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-39|Next → Spam Filter (Bag of Words)]]