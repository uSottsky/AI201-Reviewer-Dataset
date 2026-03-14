# Constraint Propagation

```python
function AC-3(csp) returns false if an inconsistency is found and true otherwise
    queue = a queue of arcs, initially all the arcs in csp
    while queue is not empty do
        (Xi, Xj) = POP(queue)
        if REVISE(csp, Xi, Xj) then
            if size of Di == 0 then return false
            for each Xk in NEIGHBORS(Xi) - {Xj} do
                add (Xk, Xi) to queue
    return true

function REVISE(csp, Xi, Xj) returns true iff we revise the domain of Xi
    revised = false
    for each x in Di do
        if no value y in Dj allows (x,y) to satisfy the constraint between Xi and Xj then
            delete x from Di
            revised = true
    return revised
    
```

22/27

---

**Navigation**
[[L4-Slide-21|Previous ← Arc Consistency (Trace 2)]]
[[L4-Slide-23|Next → Exploiting Problem Structure]]