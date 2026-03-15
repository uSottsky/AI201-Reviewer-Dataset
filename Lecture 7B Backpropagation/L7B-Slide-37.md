# Training Set Size for Good Generalization

Consider a binary classifier neural network containing a single hidden layer where
* M denotes the number of hidden neurons, W the total number of synaptic weights in the network
* $\epsilon$ denotes the fraction of errors permitted on the test set

The network will provide good generalization if these conditions are met (Baum & Haussler, 1989):
* fraction of errors made on the training set is less than $\frac{\epsilon}{2}$
* number of examples, N, used in training is
# $N\ge\frac{32W}{\epsilon}ln(\frac{32M}{\epsilon})$
(worst-case formula for estimating the training set size)

In practice, all we need for good generalization is the condition
# $N\ge\frac{W}{\epsilon}$

with an error of 10%, the number of training examples should approximately be 10 times the number of synaptic weights in the network


37/39

---
**Navigation**
[[L7B-Slide-36|Previous ← Generalization]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-38|Next → When to use MLP?]]