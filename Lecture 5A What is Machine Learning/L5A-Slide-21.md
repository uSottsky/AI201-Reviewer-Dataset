# Model Selection

Generalization error is approximated by computing the misclassification rate on a large independent test set not used during model training.

![[Pasted image 20260315165135.png]]
> Reference: Slide 21 - Graph showing Misclassification rate vs 'K' (model complexity). It illustrates a U-shaped curve where test error dips at an optimal K and rises as the model overfits, while train error consistently drops.

* U-shaped curve: complex models overfit, simple models underfit
* pick value with minimum error on test set
* algorithm should not see test set during training so it cannot choose the model with right complexity

21/25

---
**Navigation**
[[L5A-Slide-20|Previous ← Model Selection]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-22|Next → Data Partitioning]]