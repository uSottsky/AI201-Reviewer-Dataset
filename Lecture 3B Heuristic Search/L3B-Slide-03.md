# Heuristic Search

Blind search methods are, in most cases, very inefficient. Heuristic search methods find solutions more efficiently using problem-specific knowledge.

The GENERAL-SEARCH algorithm previously described implements the various blind search strategies by changing the order in which the nodes are expanded.

* done by modifying the queuing function
* only place where knowledge can be incorporated is in the queuing function

Problem-specific knowledge is embodied in a function that measures the desirability of expanding a node. Call this the evaluation function.

3/25

---
**Navigation**
[[L3B-Slide-02|Previous ← Outline]]
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]
[[L3B-Slide-04|Next → Best-First Search Strategy]]