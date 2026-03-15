# KNN


* memory-based learning / instance-based learning
* Euclidean metric often used
* induces a **Voronoi tesselation** of the training points


![[Pasted image 20260315164657.png]]
> Reference: Slide 12 - A 2D Voronoi Tesselation plot separating data points into distinct geometric regions based on distance.

* KNN: simple but suffers from curse of dimensionality

**Voronoi Tesselation:** partitioning of space that associates a region $V(x_{i})$ with each point $X_{i}$ in such a way that all points in $V(x_{i})$ are closer to $X_{i}$ than to any other point.

Predicted label is the label of the training point within the Voronoi cell.

12/25

---
**Navigation**
[[L5A-Slide-11|Previous ← K Nearest Neighbor (KNN) Classifier]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-13|Next → Curse of Dimensionality]]