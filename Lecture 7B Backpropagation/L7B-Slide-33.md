# Heuristics for Making the BP Algorithm Perform Better


**Initialization**
* randomize synaptic weights to values that are uniformly distributed within the interval $[-2.4/F_{i},+2.4/F_{i}]$ where $F_{i}$ is the fan-in (total number of inputs) of neuron i

**Maximizing Information Content**
* randomization of examples presented to the MLP from one epoch to next ensures that the successive samples in an epoch rarely belong to the same class

**Learning from Hints**
* include information such as invariance properties, symmetries or any other knowledge about the input-output mapping we want to achieve

**Learning Rates**
* learning rate should be inversely proportional to the square root of synaptic connections made to that neuron


33/39

---
**Navigation**
[[L7B-Slide-32|Previous ← Heuristics (Data Normalization)]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-34|Next → Decision Rule]]