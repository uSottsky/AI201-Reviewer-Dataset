# Cross-Validation (CV)

![[Pasted image 20260315165206.png]]
> Reference: Slide 23 - Diagram showing 5 runs of K-fold validation. The dataset is split into 5 blocks; in each run, one block (highlighted in red) is held out for testing while the others are used for training.

**K-fold Validation**
Split training data into $K$ equal size subsamples (folds) then for each fold $k \in \{1, \dots, K\}$, train on all the folds but the $k$-th and test on the $k$-th in a round robin fashion. Compute the error averaged over all the folds.

**Leave-one Out Cross-Validation (LOOCV)**
Train on all cases except for $i$ and test on $i$. Repeat $N$ times.

23/25

---
**Navigation**
[[L5A-Slide-22|Previous ← Data Partitioning]]
[[L5A-0-Table-of-Contents|↑ Lecture 5A TOC]]
[[L5A-Slide-24|Next → No Free Lunch Theorem]]