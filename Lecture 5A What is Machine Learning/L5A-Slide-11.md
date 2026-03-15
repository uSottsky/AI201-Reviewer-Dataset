# K Nearest Neighbor (Non-parametric) Classifier

![[Pasted image 20260315020923.png]]
> Reference: Slide 11 - Diagram showing points labeled '0' (blue) and '1' (red), with test points $X_1$ and $X_2$ pointing to their nearest neighbors to determine classification.

KNN classifies a test point $x$ by looking at the labels of $K$ points in the training set that are nearest to the test point, i.e.,
$$p(y=c|x,\mathcal{D},K) = \frac{1}{K} \sum_{i \in N_{k}(x,\mathcal{D})} \mathbb{I}(y_{i}=c)$$

where $N_{k}(x,\mathcal{D})$ are the indices of the $K$ nearest points to $x$ in $\mathcal{D}$ and $\mathbb{I}(e)$ is the indicator function defined as:
$$
\mathbb{I}(e) = \begin{cases} 
1 & \text{if } e \text{ is true} \\ 
0 & \text{if } e \text{ is false} 
\end{cases}
$$

11/25

---
**Navigation**
[[L5A-Slide-10|Previous ← Parametric vs Non-Parametric Models]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-12|Next → Voronoi Tesselation]]