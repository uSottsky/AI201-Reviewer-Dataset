# Search for Solutions

### The General Search Algorithm
```python
function GENERAL-SEARCH(problem, strategy) returns a solution, or failure
    initialize the search tree using the initial state of problem
    loop do
        if there are no candidates for expansion then return failure
        choose a leaf node for expansion according to strategy
        if the node contains a goal state then return the corresponding solution
        else expand the node and add the resulting nodes to the search tree
```

23/41

---

**Navigation**
[[L3A-Slide-22|Previous ← Nodes vs States]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-24|Next → Node Data Structures]]