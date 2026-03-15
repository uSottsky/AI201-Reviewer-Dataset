# M Class Bayesian Classifier

**General M Class Bayesian Classifier**

For a classification task with M classes, $\omega_1, \omega_2, \dots, \omega_m$, an unknown pattern $x$ is assigned to class $\omega_i$ if

$$
P(\omega_i|x) > P(\omega_j|x) \quad \forall j \neq i
$$

This choice minimizes the classification error probability.

**Bayes Error Rate**: classification error rate of the Bayes classifier

The Bayes Error Rate is the best possible error rate of any classifier over the distribution of all examples.

- no other classifier using the same parameter space and the same prior knowledge can outperform the Bayes Optimal Classifier on the average

**Two types of Minimization**
1. Minimize Classification Errors
2. Minimize Risk

---

12/44

[[L5B-Slide-11|Previous ← Bayes Classifier is Optimal]]
[[L5B-0-Table-of-Contents|↑ Lecture 5B TOC]]
[[L5B-Slide-13|Next → Risk Minimization]]