# Problem Types

### Search
A search problem consists of:
1. Initial State, Goal State(s), all other possible States (State Space)
2. **Operators** - set of possible actions available to the agent
3. **Goal Test** - determines whether a state is a goal state
4. **Path Cost** - a function that assigns a cost to a path

**Example: 8-Puzzle**
![[Pasted image 20260314131550.png]]
* **States**: a state description specifies the location of each of the eight tiles in one of the nine squares.
* **Operators**: blank moves left, right, up, or down
* **Goal Test**: Does the state match the goal configuration
* **Path Cost**: each step costs 1, so the path cost is just the length of the path

15/41

---
**Navigation**
[[L3A-Slide-14|Previous ← Exploratory Problem]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-16|Next → 8-Queens Formulation]]