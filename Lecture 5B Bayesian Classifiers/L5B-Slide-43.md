# Spam Filter: Laplace and Lambda Smoothing

**Problem:** one of the terms of the product is zero $\Rightarrow$ entire product is zero.
A word that does not occur in a document class (spam or ham) in the training data does not mean that it will never appear in any document of that class.

**Laplace Smoothing (add one smoothing):**
$$P(x_{i}|\omega=S) = \sum_{D\in D_{spam}} \frac{\# \text{ of times word } x_{i} \text{ is observed in } D + 1}{\text{total } \# \text{ of words in documents belonging to spam class } + \text{ vocabulary size}}$$

**Lambda Smoothing:**
$$P(x_{i}|\omega=S) = \sum_{D\in D_{spam}} \frac{\# \text{ of times word } x_{i} \text{ is observed in } D + \lambda}{\text{total } \# \text{ of words in documents belonging to spam class } + (\lambda \cdot \text{vocabulary size})}$$

---
**Navigation**
[[L5B-Slide-42|Previous ← Spam Filter: Classification Calculation]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-44|Next → References]]