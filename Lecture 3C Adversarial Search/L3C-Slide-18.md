# Alpha-Beta Pruning

```python
function MAX-VALUE(game, state, α, β) returns a (utility, move) pair
    if game.IS-TERMINAL(state) then return game.UTILITY(state, player), null
    v = -∞
    for each a in game.ACTIONS(state) do
        v2, a2 = MIN-VALUE(game, game.RESULT(state, a), α, β)
        if v2 > v then
            v, move = v2, a
            α = MAX(α, v)
        if v >= β then return v, move
    return v, move

function MIN-VALUE(game, state, α, β) returns a (utility, move) pair
    if game.IS-TERMINAL(state) then return game.UTILITY(state, player), null
    v = +∞
    for each a in game.ACTIONS(state) do
        v2, a2 = MAX-VALUE(game, game.RESULT(state, a), α, β)
        if v2 < v then
            v, move = v2, a
            β = MIN(β, v)
        if v <= α then return v, move
    return v, move

```

Similar to Minimax, except that bounds are maintained in the variables $\alpha$ and $\beta$ which are used to cut off search when a value is outside the bounds.

18/34

---

**Navigation**
[[L3C-Slide-17|Previous ← Alpha and Beta Definitions]]
[[L3C-0-Table-of-Contents|↑ Lecture 3C TOC]]
[[L3C-Slide-19|Next → Heuristic Alpha-Beta Tree Search]]