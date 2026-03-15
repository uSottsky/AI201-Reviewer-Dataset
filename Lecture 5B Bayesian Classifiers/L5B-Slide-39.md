# Spam Filter (Bag of Words)

**Spam Filter** - falls under the general category of text classification.
Document $D$ - represented as a sequence of words $x_{1},x_{2},...,x_{d}$.

Assumption: words are independent of each other ("bag of words" model):
$$P(D) = P(x_{1},x_{2},...,x_{d})$$
$$P(D) = \prod_{i=1}^{d}P(x_{i})$$

Probability of Spam Document, S:
$$P(x_{1},x_{2},...,x_{d}|\omega=S) = \prod_{i=1}^{d}P(x_{i}|\omega=S)$$

Probability of Ham Document, H:
$$P(x_{1},x_{2},...,x_{d}|\omega=H) = \prod_{i=1}^{d}P(x_{i}|\omega=H)$$

---
**Navigation**
[[L5B-Slide-38|Previous ← The Naive Bayes Classifier]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-40|Next → Spam Filter (MLE)]]