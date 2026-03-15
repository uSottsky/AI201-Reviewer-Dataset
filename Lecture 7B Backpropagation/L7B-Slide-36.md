# Generalization


A network generalizes well when the input-output mapping produced by the network is correct for input-output patterns never used in training the network (test set).

Learning process may be viewed as a "curve-fitting" problem
* generalization results from good nonlinear interpolation of training data
* overfitting leads to poor generalization
* when a neural network learns too many input-output relations, it may memorize the training data and therefore sacrifice its generalization ability
* "memorization" implies that the input-output mapping computed by the network is not "smooth"

Generalization is influenced by the following factors:
1. size and efficiency of the training set
2. architecture of the network
3. physical complexity of the problem

**Generalization Issues**
1. for a fixed architecture, determine the size of the training set needed for good generalization to occur.
2. for a given training set (of fixed size), determine the best architecture for achieving good generalization.


36/39

---
**Navigation**
[[L7B-Slide-35|Previous ← Convergence]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-37|Next → Training Set Size]]