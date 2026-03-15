# Curse of Dimensionality

Consider applying a KNN classifier to data where the inputs are uniformly distributed in a D-dimensional unit cube.
* **1-D:** 10 training points to cover 10% of the "volume"
* **2-D:** $10^{2}$ training points to cover 10% of the volume
* **N-D:** $10^{N}$ training points to cover 10% of the hypervolume

To combat curse of dimensionality, we make assumptions about the nature of the distribution ($p(y|x)$ for supervised learning or $p(x)$ for unsupervised learning).

Assumptions are known as **inductive bias**:
* can be in the form of a statistical model with a fixed number of parameters (parametric model)

13/25

---
**Navigation**
[[L5A-Slide-12|Previous ← Voronoi Tesselation]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-14|Next → Bernoulli Distribution]]