# Model Selection

**Choices:** models of varying complexity (KNN, logistic regression, etc.)
How do we choose the "right" model ?

Define the misclassification rate on the training set for each method:
$$err(f,\mathcal{D}) = \frac{1}{N} \sum_{i=1}^{N} \mathbb{I}(f(x_{i}) \ne y_{i})$$
where $f(x)$ is the classifier.

Define **generalization error** as the misclassification rule when averaged over future data.

20/25

---
**Navigation**
[[L5A-Slide-19|Previous ← Underfitting (KNN)]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-21|Next → Generalization Error]]