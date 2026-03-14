# Problem Types
![[Pasted image 20260314131208.png]]
### 8-Queens
8-Queens has two formulations:
1. **incremental formulation** - involves placing queens one by one
2. **complete state formulation** - all 8 queens on the board and move them around

**One possible incremental formulation**:
* **States**: arrangement of 0 to 8 queens on board with none attacked
* **Operators**: place a queen in the left-most empty column such that it is not attacked by any other queen

**One possible complete state formulation**:
* **States**: arrangements of 8 queens, one in each column
* **Operators**: move any attacked queen to another square in the same column

16/41

---
**Navigation**
[[L3A-Slide-15|Previous ← Components of a Search Problem]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-17|Next → 8-Queens Analysis]]