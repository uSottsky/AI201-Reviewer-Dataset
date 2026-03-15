# Spam Filter (MLE)

Use Bayes' Rule:
$$P(\omega|x_{1},x_{2},...,x_{d}) = \frac{P(x_{1},x_{2},...,x_{d}|\omega)P(\omega)}{\sum_{\omega}P(x_{1},x_{2},...,x_{d}|\omega)P(\omega)}$$

**Bag of Words Feature Independence Assumption:**
$$P(\omega|x_{1},x_{2},...,x_{d}) = \frac{\prod_{i=1}^{d}P(x_{i}|\omega)P(\omega)}{\sum_{\omega}\prod_{i=1}^{d}P(x_{i}|\omega)P(\omega)}$$

**Maximum Likelihood Estimation:**
$$P(x_{i}|\omega=S) = \sum_{D\in D_{spam}} \frac{\# \text{ of times word } x_{i} \text{ is observed in } D}{\text{total number of words in documents belonging to spam class}}$$

$$P(x_{i}|\omega=H) = \sum_{D\in D_{ham}} \frac{\# \text{ of times word } x_{i} \text{ is observed in } D}{\text{total number of words in documents belonging to ham class}}$$

---
**Navigation**
[[L5B-Slide-39|Previous ← Spam Filter (Bag of Words)]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-41|Next → Spam Filter: Training Set Example]]