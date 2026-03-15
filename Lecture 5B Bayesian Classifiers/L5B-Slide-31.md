# Minimum Distance Classifiers

Assume equiprobable classes with the same covariance matrix. Discriminant function is:
$$g_{i}(x) = -\frac{1}{2}(x-\mu_{i})^{T}\Sigma^{-1}(x-\mu_{i})$$

$\Sigma=\sigma^{2}I$; Maximum $g_{i}(x)$ implies minimum Euclidean distance:
$$d_{e} = ||x-\mu_{i}||$$

Feature vectors are assigned to classes according to their Euclidean distances from the means.


![[Pasted image 20260315205907.png]]
> Reference: Slide 31 - Graph showing two circular distributions with a straight line separating them precisely in the middle.


---
**Navigation**
[[L5B-Slide-30|Previous ← Equal Covariance Matrices]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-32|Next → Mahalanobis Distance]]