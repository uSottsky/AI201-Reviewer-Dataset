# CSP as Search

```python
function BACKTRACKING-SEARCH(csp) returns a solution or failure
    return BACKTRACK(csp, {})

function BACKTRACK(csp, assignment) returns a solution or failure
    if assignment is complete then return assignment
    var = SELECT-UNASSIGNED-VARIABLE(csp, assignment)
    for each value in ORDER-DOMAIN-VALUES(csp, var, assignment) do
        if value is consistent with assignment then
            add {var = value} to assignment
            inferences = INFERENCE(csp, var, assignment)
            if inferences != failure then
                add inferences to csp
                result = BACKTRACK(csp, assignment)
                if result != failure then return result
                remove inferences from csp
            remove {var = value} from assignment
    return failure
```

15/27

---

**Navigation**
[[L4-Slide-14|Previous ← Backtracking Search Concept]]
[[L4-0-Table-of-Contents|↑ Lecture 4 TOC]]
[[L4-Slide-16|Next → Improving Backtracking]]