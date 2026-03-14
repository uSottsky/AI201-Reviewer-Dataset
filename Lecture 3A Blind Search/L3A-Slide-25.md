# Search for Solutions

* **fringe or frontier** - a collection of nodes waiting to be expanded; best implemented as a queue for efficiency

### Queue Operations
* **MAKE-QUEUE(Elements)** creates a queue with the given elements.
* **EMPTY? (Queue)** returns true only if there are no elements in the queue.
* **REMOVE-FRONT(Queue)** removes the element at the front of the queue and returns it.
* **QUEUING-FN(Elements, Queue)** inserts a set of elements into the queue; how this is done is dependent on the search algorithm.

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


25/41

---

**Navigation**
[[L3A-Slide-24|Previous ← Node Data Structures]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-26|Next → Search Strategy Evaluation]]