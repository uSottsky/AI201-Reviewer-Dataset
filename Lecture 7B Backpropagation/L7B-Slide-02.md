# Examples of Supervised Learning Algorithms:

* Least Mean Square (LMS) Algorithm - single neuron
* Backpropagation Algorithm
    * for the Multilayer Perceptron (MLP) Neural Network
    * generalization of the LMS Algorithm

### Error-Correction Learning
Let a stimulus input vector $x(n)$ be applied to the neural network in which neuron k is embedded
* forward propagate: neuron will generate an output (actual response), $y_{k}(n)$.
* let $d_{k}(n)$ be the desired response or target response for neuron k. The error signal is the difference between the target response, $d_{k}(n)$ and the actual response $y_{k}(n)$:

# $e_{k}(n)=d_{k}(n)-y_{k}(n)$


objective of error-correction learning is to minimize a cost function based on $e_{k}(n)$


2/39

---
**Navigation**
[[L7B-Slide-01|Previous ← Title]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-03|Next → Model of a Neuron]]