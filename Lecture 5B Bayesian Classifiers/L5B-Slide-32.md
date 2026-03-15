# Mahalanobis Distance



Nondiagonal $\Sigma$: Maximum $g_{i}(x)$ implies minimum Mahalanobis distance ($\Sigma^{-1}$ norm)
$$d_{m} = \sqrt{(x-\mu_{i})^{T}\Sigma^{-1}(x-\mu_{i})}$$

Covariance matrix is symmetric and can be diagonalized by the unitary transform $\Sigma=\Phi\Lambda\Phi^{T}$ where $\Phi^{T}=\Phi^{-1}$.
* $\Lambda$ is a diagonal matrix whose elements are the eigenvalues of $\Sigma$.
* $\Phi$ has for its columns the corresponding orthonormal eigenvectors of $\Sigma$, i.e., $\Phi=[v_{1},v_{2},...,v_{l}]$. 

This gives rise to:
$$\frac{(x_{1}^{\prime}-\mu_{i1}^{\prime})^{2}}{\lambda_{1}} + ... + \frac{(x_{l}^{\prime}-\mu_{il}^{\prime})^{2}}{\lambda_{l}} = c^{2}$$



![[Pasted image 20260315210053.png]]
> Reference: Slide 32 - Graph showing two elliptical distributions with a decision line that is NOT perpendicular to the line connecting their centers.


All points having the same Mahalanobis distance from a specific mean are located on an ellipse.
* decision line is no longer orthogonal to the line segment connecting the means

---
**Navigation**
[[L5B-Slide-31|Previous ← Minimum Distance Classifiers]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-33|Next → LDA and QDA]]