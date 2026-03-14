# Game Playing in AI

### Base-Level/Meta-Level Trade-Off:
For many heuristic search problems, the heuristic function could be so complicated that computing it requires a long time.
* time spent in calculating a complicated heuristic function takes away time for expanding nodes
* time spent evaluating the heuristic function in order to select a node for expansion must be recovered by a corresponding reduction in the size of the search space explored

**Base-Level Activity** - effort spent trying to solve the problem
**Meta-Level Activity** - effort spent in deciding what to do

**Base-Level/Meta-Level Trade-Off:**
Time spent at the meta-level must be recovered by corresponding reductions in the amount of time required to solve the problem at the base-level.

 
6/34

---
**Navigation**
[[L3C-Slide-05|Previous ← Time Limits and Heuristics]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-07|Next → Perfect Decisions in Two-Person Games]]