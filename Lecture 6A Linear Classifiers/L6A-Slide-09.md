# Linear Discriminant Functions and Decision Hyperplanes

> [!NOTE] Image Needed
> Reference: Slide 9 - Geometric representation of a decision hyperplane in 2D space showing the normal weight vector $w$, perpendicular distance $d$ from the origin, and threshold $w_0$.

Consider 2-class linear discriminant function. Decision hyperplane in $l$-dimensional feature space is a hyperplane:
$$g(x) = w^T x + w_0 = 0$$
where $w = [w_1, w_2, ..., w_l]^T$; weight vector $w_0$: threshold.

For any two points $x_A$, $x_B$ on the decision hyperplane:
$$0 = w^T x_A + w_0 = w^T x_B + w_0 \Rightarrow w^T(x_A - x_B) = 0$$
Difference vector $x_A - x_B$ lies on decision hyperplane therefore vector $w$ is orthogonal to the decision hyperplane.

$$d = \frac{|w_0|}{\sqrt{w_1^2 + w_2^2}}$$
$$z = \frac{|g(x)|}{\sqrt{w_1^2 + w_2^2}}$$
where $|g(x)|$ is the Euclidean distance of the point $x$ from the decision hyperplane.

![[Pasted image 20260315214629.png]]
Distance $d$, from a point $(x_0, y_0)$ to a line $ax + by + c = 0$:
$$d = \frac{|ax_0 + by_0 + c|}{\sqrt{a^2 + b^2}}$$

---
**Navigation**
[[L6A-Slide-08|Previous ← Linear Separability]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-10|Next → Computing Unknown Parameters]]