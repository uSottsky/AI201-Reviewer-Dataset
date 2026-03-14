# Heuristic Search

### Best-First Search Strategy
Orders the nodes so that the one with the lowest evaluation is expanded first.
### The General Search Algorithm
```python
function GENERAL-SEARCH(problem, QUEUING-FN) returns a solution, or failure
    nodes = MAKE-QUEUE(MAKE-NODE(INITIAL-STATE[problem]))
    loop do
        if nodes is empty then return failure
        node = REMOVE-FRONT(nodes)
        if GOAL-TEST[problem] applied to STATE(node) succeeds then return node
        nodes = QUEUING-FN(nodes, EXPAND(node, OPERATORS[problem]))
```

2 Approaches:

- expand first the node closest to the goal (Greedy Search) 
- expand the node on the path with the least-cost solution (A ∗ )
- 
4/25

---
**Navigation**
[[L3B-Slide-03|Previous ← Heuristic Search Basics]]
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]
[[L3B-Slide-05|Next → Greedy Search]]