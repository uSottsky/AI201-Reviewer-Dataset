# Mean Square Error Estimation

### Mean Square Error Estimation (Geometric View)

![[Pasted image 20260315215315.png]]
> Reference: Slide 21 - 3D geometric view showing a vector $y$ in space and its orthogonal projection $w^T x$ onto the subspace defined by the input variables $x_i$, leaving a perpendicular error vector $y - w^T x$.

Encode random variables as points in vector space. The expectation operation $E[xy]$ between 2 random variables satisfies the properties of the inner product.

The quantity $w^T x = w_1 x_1 + w_2 x_2 + \cdots + w_l x_l$ is a linear combination of vectors and thus lies in the subspace defined by the $x_i$.
We approximate $y$ by this linear combination and the resulting error is $y - w^T x$.

The equation $$\hat{w} = \arg \min_w J(w)$$ states that the minimum MSE solution results if the error is orthogonal to each $x_i$.
It is orthogonal to the vector subspace spanned by $x_i, i=1,2,...,l$.
$y$ is approximated by its orthogonal projection on the subspace.

---
**Navigation**
[[L6A-Slide-20|Previous ← Minimizing J(w)]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-22|Next → Multiclass Case]]