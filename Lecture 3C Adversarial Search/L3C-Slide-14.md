# Mini-Max

### Imperfect Decisions
* has time limit
* memory space is also limited

**How do humans play games?**
* don't analyze it all the way to the end
* look a few moves ahead, evaluate the nonterminal position and "back-up" the value we have formed
* minimax still applies

**We modify minimax in the following way:**
1. replace utility function by an **evaluation function**
   * evaluation function - returns an estimate of pay-off value
2. replace terminal test by a **cut-off test**

Minimax computes the optimal playing strategy but does so inefficiently since it generates a complete tree and then computes and backs up static evaluation function.

 
14/34

---
**Navigation**
[[L3C-Slide-13|Previous ← Chess: Rules & Objective]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-15|Next → Alpha-Beta Pruning Example]]