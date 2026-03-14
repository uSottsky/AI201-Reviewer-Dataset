---

---
---
## Model-based Reflex Agent

- reflex agent but with an **internal state** that keeps track of the part of the world it cannot see now. 

![[Pasted image 20260314020821.png]]
```python 
function MODEL-BASED-REFLEX-AGENT(percept) returns an action 
		persistent: state, the agent's current conception of the world state
		transition_model, a description of how the next state depends on 
			the current state and action 
		sensor_model, a description of how the current world state is reflected 
			in the agent's percepts 
		rules, a set of condition-action rules 
		action, the most recent action, initially none
state ← UPDATE-STATE(state, action, percept, transition_model, sensor_model) action ← RULE-MATCH(state, rules) 
return action
```

- maintains internal state information to distinguish between world states that generate the same perceptual input but requiring different actions
- uses perceptual history as basis of its actions

**Two types of information are needed by this type of agent:**

- information about how the world changes independently of the agent (must be built-in)
- information about how the agent's actions affect the world

13/27

----
Navigation
[[L2-Slide-12|Previous ← Simple Reflex Agent]]
[[L2-0-Table-of-Contents]]
[[L2-Slide-14|Next → Model-based Reflex Agent (continued)]]