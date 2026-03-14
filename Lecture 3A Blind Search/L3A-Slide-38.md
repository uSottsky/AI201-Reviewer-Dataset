# Blind Search: Iterative Deepening Search 

**IDS**: 
* complete since it can find a solution no matter how deep it is 
* optimal since the shallowest solution is always found 

**Overhead of multiple expansion**: 
* is small especially for tree with high branching factor 
* even for binary trees (b=2), IDS only takes twice as long as a complete BFS 

Time complexity is $\mathcal{O}(b^{d})$ and space complexity is $\mathcal{O}(bd)$ if solution is found at depth d. 

**Iterative Deepening Search is the preferred search method when there is a large search space and the depth of the solution is unknown.**

38/41

--- 
**Navigation** 
[[L3A-Slide-37|Previous ← IDS Algorithm Implementation]] 
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-39|Next → Bidirectional Search]]