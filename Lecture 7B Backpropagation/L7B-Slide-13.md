# Backpropagation Algorithm Derivation

### Output Neuron

![[Pasted image 20260314203454.png]]
> Reference: Slide 13 - Diagram of an output neuron $j$, showing inputs, summing junction, desired output $d_j(n)$, and error calculation $e_j(n)$.

Assume that the network in is the training phase. Start by presenting the $n$-th training input pattern $x(n)$ to the network.
Neuron $j$ has same number of inputs as the number of neurons in the previous layer plus one fixed input of +1 corresponding to the trainable weight bias $w_{j0}(n)$.

For output **neuron j**,
# $e_{j}(n)=d_{j}(n)-y_{j}(n)$                                               (5)

where
# * $e_{j}(n)$: error signal
# * $d_{j}(n)$: desired response
# * $y_{j}(n)$: output signal


13/39

---
**Navigation**
[[L7B-Slide-12|Previous ← Conventions and Notations]]
[[AI 201 - Artificial Intelligence/Lecture 7B Backpropagation/L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-14|Next → Cost Function (Error)]]