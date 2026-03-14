# Backpropagation Algorithm Derivation

### Logistic Function Nonlinearity


Computing for the weight update for each neuron requires derivative of the activation function $\varphi(\cdot)$.
![[Pasted image 20260314212335.png]]
> Reference: Slide 23 - Graph of the Logistic function showing different slopes.


The logistic activation function
# $\varphi(v_{j}(n))=\frac{1}{1+exp(-av_{j}(n))} \quad a>0$

has a derivative
# $\varphi^{\prime}(v_{j}(n))=\frac{a~exp(-av_{j}(n))}{[1+exp(-av_{j}(n))]^{2}}$
# $\varphi^{\prime}(v_{j}(n))=a~\varphi(v_{j}(n))[1-\varphi(v_{j}(n))]$                                (13)


23/39

# Supplemental: Deriving the Logistic Activation Function using the Quotient Rule (Slide 23)

Slide 23 shows the derivative of the Logistic Activation function. To make the math easier to follow, let's use the exact `exp()` notation from the slide and break down the calculus step-by-step using the **Quotient Rule**, just like you would learn in a high school calculus class.

### The Equation
The logistic activation function, given a slope parameter $a$ and an internal activity $v_j(n)$, is defined as:
# $$\varphi(v_j(n)) = \frac{1}{1 + \exp(-a v_j(n))}$$

We want to find its derivative with respect to $v_j(n)$. To keep the notation clean during the calculus steps, let's just use $v$ instead of $v_j(n)$:
# $$\varphi(v) = \frac{1}{1 + \exp(-av)}$$
### Step 1: Set up the Quotient Rule
In calculus, the Quotient Rule tells us how to take the derivative of a fraction. If you have a function that is a "top" divided by a "bottom" $\left( \frac{\text{Top}}{\text{Bottom}} \right)$, the rule is:
Let's identify our Top and Bottom pieces:
* **Top:** $1$
* **Bottom:** $1 + \exp(-av)$
# $$\text{Derivative} = \frac{(\text{Derivative of Top} \cdot \text{Bottom}) - (\text{Top} \cdot \text{Derivative of Bottom})}{(\text{Bottom})^2}$$
### Step 2: Find the derivatives of the Top and Bottom
Now we take the derivative of both pieces separately.

**Derivative of the Top:**
The top is just the number $1$. The derivative of any constant number is always $0$.
* **Derivative of Top = $0$**

**Derivative of the Bottom:**
The bottom is $1 + \exp(-av)$.
* The derivative of the $1$ is $0$.
* To find the derivative of $\exp(-av)$, we use the Chain Rule. We take the derivative of the `exp` function (which stays the exact same) and multiply it by the derivative of its "inside" (the exponent $-av$).
* The derivative of $-av$ with respect to $v$ is just $-a$.
* **Derivative of Bottom = $-a \cdot \exp(-av)$**

---

### Step 3: Plug everything into the Quotient Rule
Now we substitute our four pieces back into the Quotient Rule formula from Step 1:

# $$\varphi^{\prime}(v) = \frac{(0 \cdot [1 + \exp(-av)]) - (1 \cdot [-a \cdot \exp(-av)])}{[1 + \exp(-av)]^2}$$

Let's simplify the top part of that fraction:
* $0$ multiplied by anything is $0$, so the first part disappears.
* We are left with $-(1 \cdot [-a \cdot \exp(-av)])$.
* The two negative signs cancel each other out ($-\times - = +$), leaving us with a positive $a \cdot \exp(-av)$.

This gives us the first intermediate derivative shown on Slide 23:
# $$\varphi^{\prime}(v) = \frac{a \exp(-av)}{[1 + \exp(-av)]^2}$$

### Step 4: The Algebraic Trick (Simplifying to the final form)
While the result in Step 3 is correct, it looks messy. In neural networks, we want to calculate things as fast as possible. Notice that the original function $\varphi(v)$ is hiding inside this result. We can use algebra to pull it out.

First, let's split the fraction from Step 3 into two separate fractions multiplied together:

Look closely at the first fraction. It is exactly our original activation function! We can replace it with $\varphi(v)$:
# $$\varphi^{\prime}(v) = a \cdot \left( \frac{1}{1 + \exp(-av)} \right) \cdot \left( \frac{\exp(-av)}{1 + \exp(-av)} \right)$$$$\varphi^{\prime}(v) = a \cdot \varphi(v) \cdot \left( \frac{\exp(-av)}{1 + \exp(-av)} \right)$$
### Step 5: Formatting the Second Fraction
We want to get rid of the `exp` in the second fraction too. We can do a clever high school algebra trick: add $1$ and subtract $1$ in the top part of the fraction. Adding $1 - 1$ is just adding $0$, so it doesn't change the value of the fraction, but it allows us to rearrange it.

# $$\frac{\exp(-av)}{1 + \exp(-av)} \quad \rightarrow \quad \frac{1 + \exp(-av) - 1}{1 + \exp(-av)}$$

Now, we can split this single fraction into two smaller fractions:
# $$\frac{1 + \exp(-av)}{1 + \exp(-av)} - \frac{1}{1 + \exp(-av)}$$

* The first part is something divided by itself, which simplifies to exactly $1$.
* The second part is exactly our original activation function, $\varphi(v)$!

So, the whole messy fraction simply becomes:
# $$1 - \varphi(v)$$

### Step 6: The Final Result
Substitute this beautifully simplified piece back into our equation from Step 4. Bringing back the proper $v_j(n)$ notation, we arrive at the exact final formula shown on Slide 23:

# $$\varphi^{\prime}(v_j(n)) = a \cdot \varphi(v_j(n)) \cdot [1 - \varphi(v_j(n))]$$

*(Why do this? Because during coding, if the neuron already calculated its output $\varphi(v)$, it doesn't have to do the expensive `exp()` math again to find its derivative. It just multiplies its output by 1 minus its output!)**

---
# **Navigation**
[[L7B-Slide-22|Previous ← The Generalized Delta Rule]]
[[L7B-0-Table-of-Contents|↑ Lecture 7B TOC]]
[[L7B-Slide-24|Next → Local Gradient (Logistic)]]