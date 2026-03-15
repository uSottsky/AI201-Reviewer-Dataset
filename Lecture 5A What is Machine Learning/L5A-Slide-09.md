# Probabilistic Approach to Classification

Let $p(y|x,\mathcal{D})$: probability distribution over possible labels given the input vector $x$ and training set $\mathcal{D}$.

**Best guess for the true label:**
$$\hat{y} = \hat{f}(x) = \arg \max_{c \in \{1,\dots,C\}} p(y=c|x,\mathcal{D})$$

* which is the most probable class label; also corresponds to the mode of the distribution $p(y|x,\mathcal{D})$.
* also known as the MAP (maximum a posteriori) estimate

9/25

---
**Navigation**
[[L5A-Slide-08|Previous ← Classification Types]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-10|Next → Parametric vs Non-Parametric Models]]