# Game Playing in AI

**Games have time limits.**
* execution efficiency is very important
* games have spurred the development of any-time algorithms

**All games are contingency problems.**
* game-playing agent must calculate a whole tree of actions where each branch deals with what the opponent will do.

**How to deal with time limit:** use techniques that allow us to ignore portions of the search tree that make no difference to the final choice.
* need heuristic evaluation functions that measure how good a position is without doing a complete search

**Purpose of heuristic function:** reduce the search space to be explored

 
5/34

---
**Navigation**
[[L3C-Slide-04|Previous ← Single-agent vs Multi-agent Games]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-06|Next → Base-Level vs Meta-Level Trade-Off]]