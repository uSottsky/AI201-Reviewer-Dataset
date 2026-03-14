# Heuristic Alpha-Beta Tree Search

### Horizon Effect and other Problems
Evaluation function gives only estimates of pay-off function.

**1. The Horizon Effect** - arises when there is a threat that appears unavoidable
* some useless moves such as a "nuisance" check could push out a threat "over the horizon" instead of directly dealing with the threat
* it is difficult to distinguish between a move that really neutralizes the threat and one that just pushes the threat over the horizon

**Proposed Solutions to the Horizon Effect:**
1. **Secondary Search** - examine search space beneath the apparently best move to see if something has in fact been pushed beyond the horizon so that an alternate move can be chosen
2. **Killer Heuristic** - if you find that a move is good for your opponent, look at this move early when considering your opponent's actions
3. combine 1 and 2 but not all instances of the horizon problem can be avoided

 
23/34

---
**Navigation**
[[L3C-Slide-22|Previous ← Cutting Off Search]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-24|Next → Quiescence and Singular Extension]]