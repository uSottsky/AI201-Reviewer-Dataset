# Diagonal Covariance Matrix with Equal Elements

Assume mutually uncorrelated features of equal variance: $E[(x_{i}-\mu_{i})(x_{j}-\mu_{j})] = \sigma^{2}\delta_{ij}$
Discriminant function becomes $g_{i}(x) = \frac{1}{\sigma^{2}}\mu_{i}^{T}x + w_{i0}$ with hyperplanes:
$$g_{ij}(x) \equiv g_{i}(x) - g_{j}(x) = w^{T}(x-x_{0}) = 0$$

where:
* $w = \mu_{i} - \mu_{j}$
* $x_{0} = \frac{1}{2}(\mu_{i}+\mu_{j}) - \sigma^{2}\ln\left(\frac{P(\omega_{i})}{P(\omega_{j})}\right)\frac{\mu_{i}-\mu_{j}}{||\mu_{i}-\mu_{j}||^{2}}$
($||\cdot||$: Euclidean norm)

decision surface is a hyperplane passing through $x_{0}$
* **if $P(\omega_{i})=P(\omega_{j})$:** $x_{0}=\frac{1}{2}(\mu_{i}+\mu_{j})$ i.e., hyperplane is the perpendicular bisector of line segment joining the means
* **if $P(\omega_{i})>P(\omega_{j})$:** hyperplane is closer to $\mu_{j}$ and area where we decide in favor of the more probable of the two classes is increased
* **for both cases:** decision hyperplane is perpendicular to the line segment connecting the two means since:
$$g_{ij} = 0 \Rightarrow w^{T}(x-x_{0}) = (\mu_{i}-\mu_{j})^{T}(x-x_{0}) = 0$$

---
**Navigation**
[[L5B-Slide-25|Previous ← Decision Hyperplanes]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-27|Next → Decision Lines Visualization]]