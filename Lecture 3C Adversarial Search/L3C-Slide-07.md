# Game Playing in AI

### Perfect Decisions in Two-Person Games
Problem (initial state, operators, goal test, path cost function)

**In games, we have the following:**
1. **initial state, $S_0$** - board configuration; whose turn to move
2. **To-Move(s)** - player whose turn it is to move for state s
3. **Actions(s)** - set of legal moves in state s
4. **IsTerminal(s)** - terminal test that checks whether game is over (terminal states = goal)
5. **Utility(s, p)** - utility function (or objective function/pay-off function) that defines the numeric value for the final outcome of the game to player p.

 
7/34

---
**Navigation**
[[L3C-Slide-06|Previous ← Base-Level vs Meta-Level Trade-Off]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-08|Next → Mini-Max Strategy]]