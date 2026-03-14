# Properties of A* Complexity

# Properties of A* Complexity

Iterative Deepening A*

```python
function IDA*(problem) returns a solution sequence
    inputs: problem, a problem
    static: f-limit, the current f- COST limit
            root, a node
    root = MAKE-NODE(INITIAL-STATE[problem])
    f-limit = f-COST(root)
    loop do
        solution, f-limit = DFS-CONTOUR(root, f-limit)
        if solution is non-null then return solution
        if f-limit = ∞ then return failure; end

function DFS-CONTOUR(node, f-limit) returns a solution sequence and a new f- COST limit
    inputs: node, a node
            f-limit, the current f- COST limit
    static: next-f, the f- COST limit for the next contour, initially ∞
    if f-COST[node] > f-limit then return null, f-COST[node]
    if GOAL-TEST[problem](STATE[node]) then return node, f-limit
    for each node s in SUCCESSORS(node) do
        solution, new-f = DFS-CONTOUR(s,f-limit)
        if solution is non-null then return solution,f-limit
        next-f = MIN(next-f, new-f); end
    return null, next-f
    
```

24/25

---
**Navigation** [[L3B-Slide-23|Previous ← Iterative Deepening A* (Korf)]]  
[[L3B-0-Table-of-Contents|↑ Lecture 3B TOC]]  
[[L3B-Slide-25|Next → End]]



