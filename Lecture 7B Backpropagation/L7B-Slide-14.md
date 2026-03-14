# Backpropagation Algorithm Derivation

### Output Neuron
Define the instantaneous value of the square error for output neuron j as $\frac{1}{2}e_{j}^{2}(n)$.

The instantaneous sum of square errors $\mathcal{E}(n)$ of the network is

# $\mathcal{E}(n)=\frac{1}{2}\sum_{j\in C}e_{j}^{2}(n)$                                     (6)

where C is the set of all output neurons of the network.

For the N input patterns in the training set, the average squared error for the entire training set is

# $\mathcal{E}_{av}=\frac{1}{N}\sum_{n=1}^{N}\mathcal{E}(n)=\frac{1}{2N}\sum_{n=1}^{N}\sum_{j\in C}e_{j}^{2}(n)$

Objective of the learning process is to adjust the weights so as to minimize the cost function $\mathcal{E}_{av}$.


14/39


# Supplemental: Deriving the Average Squared Error ($\mathcal{E}_{av}$)

The formula for $\mathcal{E}_{av}$ on Slide 14 might look intimidating, but it is just built up logically in three steps. Here is the step-by-step breakdown of how the equation comes together:

### Step 1: The Error for a Single Output Neuron
For a single output neuron $j$ at a specific training iteration $n$, the raw error signal is $e_j(n)$. 
To prevent negative errors from canceling out positive errors, we square this value. 
We also multiply it by $\frac{1}{2}$ to make the calculus cleaner later on (when we take the derivative during backpropagation, the exponent $2$ drops down and cancels out the $\frac{1}{2}$). 
* **Instantaneous squared error for one neuron:** $\frac{1}{2}e_j^2(n)$

### Step 2: The Error for the Entire Network (One Training Pattern)
A neural network usually has multiple output neurons. Let $C$ be the set of all these output neurons. 
To find the total error of the *entire network* for that single training pattern $n$, we simply sum up the individual squared errors of every output neuron.
* **Instantaneous sum of squared errors:**
  # $$\mathcal{E}(n) = \sum_{j \in C} \left( \frac{1}{2} e_j^2(n) \right) = \frac{1}{2} \sum_{j \in C} e_j^2(n)$$

### Step 3: The Average Error Across All Training Patterns
We don't just care about the network's error on one single pattern; we want to evaluate its performance across the entire training set (an epoch). If there are $N$ input patterns in the training set, we calculate the mean (average) of $\mathcal{E}(n)$ over all $N$ patterns.
* **Average squared error:**
  $$\mathcal{E}_{av} = \frac{1}{N} \sum_{n=1}^{N} \mathcal{E}(n)$$

### Step 4: Substitution and Final Formula
Finally, we substitute the definition of $\mathcal{E}(n)$ from Step 2 into the average equation from Step 3:
$$\mathcal{E}_{av} = \frac{1}{N} \sum_{n=1}^{N} \left( \frac{1}{2} \sum_{j \in C} e_j^2(n) \right)$$

By pulling the constant fraction $\frac{1}{2}$ out to the front, we get the final equation shown on the slide:
$$\mathcal{E}_{av} = \frac{1}{2N} \sum_{n=1}^{N} \sum_{j \in C} e_j^2(n)$$

**Summary of the pieces:**
* $\frac{1}{2N}$: The combined constants for averaging over $N$ patterns and the $\frac{1}{2}$ used for clean derivatives.
* $\sum_{n=1}^{N}$: Summing across all training examples in the epoch.
* $\sum_{j \in C}$: Summing across all output neurons in the network.
* $e_j^2(n)$: The squared error of a specific neuron on a specific training example.
---
# **Navigation**
[[L7B-Slide-13|Previous ← Output Neuron Error]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-15|Next → Output Neuron Activation]]

---
