# MSE and MAE

For regression problems, the aim is to minimize the **mean squared error (MSE)**:
$$MSE = \frac{1}{N} \sum_{i=1}^N (\hat{y}_i - y_i)^2$$
where $y_i$ is the correct value for target $i$ and $\hat{y}_i$ is the target's predicted value.
* puts more emphasis on larger errors more than on smaller ones
* treats positive and negative errors equally

**Mean Absolute Error (MAE)**
* less harsh to large errors
$$MAE = \frac{1}{N} \sum_{i=1}^N |\hat{y}_i - y_i|$$

---
**Navigation**
[[L6B-Slide-16|Previous ← Matthews Correlation Coefficient]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-18|Next → Pearson Correlation Coefficient]]