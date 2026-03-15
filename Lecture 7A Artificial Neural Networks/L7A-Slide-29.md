# Biological Neurons

![[Pasted image 20260316030722.png]]
> Reference: Slide 29 - Combination of the Character Recognition neural network block and the Supervised Learning block diagram from previous slides.

* vector describing the state of the environment (bit string representing the pixels of a character) is fed to both teacher and the neural network
* teacher and neural network give desired response and actual response. Difference between the two responses constitute the error signal
* error signal is used to adjust the synaptic weights of the network so as to minimize the error
* error-correction learning algorithm is employed to adjust the synaptic weights
* training process is repeated over all input-output examples until the network has been trained
* network is considered to have been trained once the average value of the error signal for the different examples is small (below a certain threshold)

---
**Navigation**
[[L7A-Slide-28|Previous ← Example: Character Recognition (Part 1)]]
[[L7A-0-Table-of-Contents|↑ Lecture 7A TOC]]
[[L7A-Slide-30|Next → Classification Capabilities of the 2 Layer Perceptron]]