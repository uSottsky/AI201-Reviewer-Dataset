# Types of Agents

## Table-Driven Agent

Store percept sequence in memory and use it as an index into a table which contains the appropriate action for all possible sequences.
![[Pasted image 20260314011721.png]]
```python
function TABLE-DRIVEN-AGENT(percept) returns an action
    persistent: percepts, a sequence, initially empty
    table, a table of actions, indexed by percept sequences, initially fully specified

    append percept to the end of percepts
    action ← LOOKUP(percepts, table)
    return action
```

**What's wrong with a Table-Driven Agent?**

- table is extremely large ($10^{123}$ entries for chess)
- it will take the designer a long time to build the table, if at all
- since table is built-in knowledge, there is no autonomy at all.
- If environment changes in a way that was not foreseen by the designer, the agent will not be able to act rationally
- even if there is a learning mechanism, it will take a very long time to learn the right value for all table entries
    

11/27

---

**Navigation**
[[L2-Slide-10|Previous ← PEAS Description]]
[[L2-0-Table-of-Contents|↑ Lecture 2 TOC]]
[[L2-Slide-12|Next → Simple Reflex Agent]]