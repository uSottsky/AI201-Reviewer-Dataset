# Monte Carlo Tree Search (MCTS)

```python
function MONTE-CARLO-TREE-SEARCH(state) returns an action
    tree = NODE(state)
    while IS-TIME-REMAINING() do
        leaf = SELECT(tree)
        child = EXPAND(leaf)
        result = SIMULATE(child)
        BACK-PROPAGATE(result, child)
    return the move in ACTIONS(state) whose node has highest number of playouts
```

- time to compute playout is linear in the depth of the game tree since only one move is taken at each choice point thus giving time for multiple playouts
- MCTS better than Alpha-Beta Search for games with high branching factor
- MCTS less vulnerable to error arising from wrong evaluation function
- Alpha-Beta Search better for games where a single move could change the entire course of the game

30/34

---

**Navigation** 
[[L3C-Slide-29|Previous ← MCTS 4-Step Process]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-31|Next → Stochastic Games (Backgammon)]]