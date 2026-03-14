# Blind Search: Iterative Deepening Search

```python
function ITERATIVE-DEEPENING-SEARCH(problem) returns a solution node or failure
    for depth = 0 to ∞ do
        result = DEPTH-LIMITED-SEARCH(problem, depth)
        if result != cutoff then return result

function DEPTH-LIMITED-SEARCH(problem, l) returns a node or failure or cutoff
    frontier = a LIFO queue (stack) with NODE(problem.INITIAL) as an element
    result = failure
    while not IS-EMPTY(frontier) do
        node = POP(frontier)
        if problem.Is-GOAL(node.STATE) then return node
        if DEPTH(node) > l then
            result = cutoff
        else if not IS-CYCLE(node) do
            for each child in EXPAND (problem, node) do
                add child to frontier
    return result

```


37/41

---

**Navigation** 
[[L3A-Slide-36|Previous ← Iterative Deepening Search (IDS)]] 
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]] 
[[L3A-Slide-38|Next → IDS Performance & Summary]]