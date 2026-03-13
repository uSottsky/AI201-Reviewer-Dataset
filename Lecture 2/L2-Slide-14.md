
---

# Model-based Reflex Agent (continued)

![[Pasted image 20260314020918.png]]

```python
function MODEL-BASED-REFLEX-AGENT(percept) returns an action
    persistent: state, the agent's current conception of the world state
    transition_model, a description of how the next state depends on the current state and action
    sensor_model, a description of how the current world state is reflected in the agent's percepts
    rules, a set of condition-action rules
    action, the most recent action, initially none

    state ← UPDATE-STATE(state, action, percept, transition_model, sensor_model)
    rule ← RULE-MATCH(state, rules)
    action ← rule.ACTION
    return action
```

**How the world evolves** requires knowledge that is encoded in the agent program:

- **transition model** of the world
- **sensor model** – how state of the world is reflected in the agent's percepts
14/27

---

Navigation 
[[L2-Slide-13|Previous ← Model-based Reflex Agent]]
[[L2-0-Table-of-Contents]] 
[[L2-Slide-15|Next → Model-based Goal-based Agent]]