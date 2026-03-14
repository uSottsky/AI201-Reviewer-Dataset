
---
# Reflex Agent

- selects action on the basis of the **current percept**, ignores percept history

![[Pasted image 20260314020802.png]]

```python
function SIMPLE-REFLEX-AGENT(percept) returns an action
    persistent: rules, a set of condition-action rules
    state ← INTERPRET-INPUT(percept)
    rule ← RULE-MATCH(state, rules)
    action ← rule.ACTION
    return action
    
```
A simple reflex agent maps percepts to actions using **condition-action rules**.

**Examples**:
- if car-in-front-is-braking then initiate-braking
- simple reflex agent looks for the rule whose condition matches the current situation (as defined by the percept) and then does the action associated with that rule

Works very efficiently but its applicability is very limited since it only uses the current percept.

12/27

---
Navigation
[[L2-Slide-11|Previous ← Table-Driven Agent]]
[[L2-0-Table-of-Contents]]
[[L2-Slide-13|Next → Model-based Reflex Agent]]


