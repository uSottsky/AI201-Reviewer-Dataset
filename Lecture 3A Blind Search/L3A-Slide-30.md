# Blind Search: Breadth-First Search

Time complexity is $\mathcal{O}(b^{d})$. Space complexity is also $\mathcal{O}(b^{d})$. For BFS, time and space complexity are both exponential.

### BFS Time and Memory Requirements
| Depth | Nodes | Time | Memory |
| :--- | :--- | :--- | :--- |
| 0 | 1 | 1 millisecond | 100 bytes |
| 2 | 111 | .1 seconds | 11 kilobytes |
| 4 | 11,111 | 11 seconds | 1 megabyte |
| 6 | $10^{6}$ | 18 minutes | 111 megabytes |
| 8 | $10^{8}$ | 31 hours | 11 gigabytes |
| 10 | $10^{10}$ | 128 days | 1 terabyte |
| 12 | $10^{12}$ | 35 years | 111 terabytes |
| 14 | $10^{14}$ | 3500 years | 11,111 terabytes |

* For BFS, execution time is a bigger problem that memory requirements.

30/41

---
**Navigation**
[[L3A-Slide-29|Previous ← BFS Implementation & Complexity]]
[[L3A-0-Table-of-Contents|↑ Lecture 3A TOC]]
[[L3A-Slide-31|Next → Uniform Cost Search (UCS)]]