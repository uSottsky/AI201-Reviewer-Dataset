# For What Problems is the MLP Appropriate?

The Backpropagation Algorithm is well-suited for problems where:
1. inputs that are represented as a vector
    - elements of the input vector may be highly correlated or independent of one another
    - input values can be any real values
2. the target function output may be
    - discrete-valued
    - real-valued
    - vector-valued having elements that are real-valued and/or discrete-valued
3. training data may contain errors
    - MLP is inherently robust to noise in training data
4. long training times are acceptable
    - training time could range from a few seconds to many hours depending on fast evaluation of the learned target function
    - training time can be very long but evaluating the learned target function value is typically very fast
5. the ability of humans to understand the learned target function is not important
    - the weights learned by the neural network are often difficult to interpret since they do not possess a meaning of their own in the eyes of the human user


38/39

---
**Navigation**
[[L7B-Slide-37|Previous ← Training Set Size]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-39|Next → References]]