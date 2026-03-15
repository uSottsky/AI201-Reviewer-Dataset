# PPV and NPV

**Positive Predictive Value (PPV)** - number of cases that actually have a disease divided by the number of cases that the classifier classifies as having a disease
$$PPV = \frac{TP}{TP+FP}$$
* indicates how probable it is that a case has a disease when the classifier has a positive/disease class as output
* how much one should believe the classifier when it indicates that the person has the disease
* for 2-class case, PPV is equal to Precision

**Negative Predictive Value (NPV)** - number of cases that actually are healthy divided by the number of cases that the classifier classifies as healthy
$$NPV = \frac{TN}{TN+FN}$$
* indicates how probable it is that a person is healthy when the classifier has a negative/health class as output
* how much one should believe the classifier when it indicates that the person is healthy

---
**Navigation**
[[L6B-Slide-08|Previous ← Specificity]]
[[L6B-0-Table-of-Contents|↑ Lecture 6B TOC]]
[[L6B-Slide-10|Next → Word of Caution on PPV and NPV]]