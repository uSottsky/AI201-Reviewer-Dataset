# Blind Search: Bidirectional Search

### 6. Bidirectional Search (Pohl, 1969)

![[Pasted image 20260314135420.png]]
> Reference: Slide 39 - Diagrams showing simultaneous forward search from "Start" and backward search from "Goal".

* agent simultaneously searches both forward from the initial state and backward from the goal.
* The search terminates when the two searches meet in the middle.

**Issues that need to be addressed**:
* when searching backwards, it is necessary to generate the predecessors successively from the goal node.
* how do you deal with problems with many possible goal states ?
* how do you generate the predecessors of a goal that is an abstract description ? (e.g. what are the predecessors of the checkmate goal in chess ?).

Time complexity is $\mathcal{O}(2b^{d/2}) = \mathcal{O}(b^{d/2})$ and space complexity is $\mathcal{O}(b^{d/2})$ if solution is found at depth d.

39/41

---
**Navigation**
[[L3A-Slide-38|Previous ← IDS Performance & Summary]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-40|Next → Bidirectional Search Algorithm]]