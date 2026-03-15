# Computing Unknown Parameters

How do we compute for the unknown parameters $w_i$, $i=0,...,l$ defining the hyperplane?

Assume two linearly separable classes $\omega_1$, $\omega_2$. Linear separability means that there exists a hyperplane $w^{*T} x + w_0^* = 0$ such that:
* $$w^{*T}x + w_0^* > 0 \quad \forall x \in \omega_1$$
* $$w^{*T}x + w_0^* < 0 \quad \forall x \in \omega_2$$

For the case where the hyperplane does not cross the origin, define extended $(l+1)$ dimensional vectors $x' \equiv [x^T, 1]^T$, $w' \equiv [w^{*T}, w_0^*]^T$.
Then $w^{*T}x + w_0^* = w'^T x'$

Let $Y$ be the subset of training vectors that are misclassified by the hyperplane. Define the following cost function:
$$J(w) = \sum_{x \in Y} (\delta_x w^T x)$$

where $\delta_x$ is chosen so that $\delta_x = -1$ if $x \in \omega_1$ and $\delta_x = +1$ if $x \in \omega_2$.
* if $x \in \omega_1$ and it is misclassified, then $w^T x < 0$ and $\delta_x < 0 \Rightarrow$ product is positive.
* If $x \in \omega_2$ and it is misclassified, then $w^T x > 0$ and $\delta_x > 0 \Rightarrow$ product is positive.
* sum is zero when $Y$ is empty set.

When cost function is zero, a solution has been found since all training feature vectors are correctly classified.

---
**Navigation**
[[L6A-Slide-09|Previous ← Linear Discriminant Functions and Decision Hyperplanes]]
[[L6A-0-Table-of-Contents|↑ Lecture 6A TOC]]
[[L6A-Slide-11|Next → The Perceptron Algorithm]]