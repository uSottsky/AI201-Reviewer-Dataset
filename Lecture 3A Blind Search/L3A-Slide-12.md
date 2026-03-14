# Problem Types

### Multiple-State Problem

![[Pasted image 20260314131500.png]]
> Reference: Slide 12 - State-transition diagram for the Vacuum World showing L, R, and S actions.

Agent in multiple-state problem:
* knows it is in one of several world states (world is not fully accessible)
* knows the effects of its actions

* agent knows it is in one of the following world states: {1,2,3,4,5,6,7,8}
* action {move-right} brings the agent to one of the states {2,4,6,8}
* agent can reason out that the action sequence {move-right, suck-dirt, move-left, suck-dirt} will make it reach a goal state from any initial state.
* world not fully accessible so agent must reason about the states it will get into

For both single-state and multiple-state problems, there is a sequence of actions that is guaranteed to bring the agent to the goal from any initial state.

12/41

---
**Navigation**
[[L3A-Slide-11|Previous ← Single-State Problem]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-13|Next → Contingency Problem]]