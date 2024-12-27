# Day 1: Calculus $\Iota$ Review

## Derivative Rules

### Power Rule

$$
\large
\frac{d}{dx} x^n = nx^{n-1}
$$

### Constant Rule

$$
\large
\frac{d}{dx} C = 0, \nobreakspace C = \text{any constant}
$$

### Sum Rule

$$
\large
\frac{d}{dx} f(x) + g(x) = f'(x) + g'(x)
$$

### Product Rule

$$
\large
\frac{d}{dx} (f(x)g(x)) = f'(x)g(x) + f(x)g'(x)
$$

### Quotient Rule

The Quotient Rule is used to find the derivative of a function that is the ratio of two differentiable functions.

If you have a function $\large f(x) = \frac{g(x)}{h(x)}$, where both $\large g(x)$ and $\large h(x)$ are differentiable, then the derivative of $\large f(x)$ is given by:

$$
\large
\frac{d}{dx} f(x) = \frac{g(x)}{h(x)} = \frac{g'(x)h(x) - g(x)h'(x)}{[h(x)]^2}
$$

Where:

- $g(x)$ - is the numerator function
- $h(x)$ is the denominator function
- $g'(x)$ is the derivative of $g(x)$
- $h'(x)$ is the derivative of $h(x)$

Remember to apply the Quotient Rule carefully, ensuring that you correctly identify and differentiate the numerator and denominator functions.

### Chain Rule

The Chain Rule is used to find the derivative of composite functions.

If you have a function $\large f(x) = g(h(x))$, where both $\large g(x)$ and $\large h(x)$ are differentiable, then the derivative of $\large f(x)$ is given by:

$$
\large
\frac{d}{dx} f(x) = \frac{d}{dx}[{g(h(x))}] = g'(h(x)) \cdot h'(x)
$$

Where:

- $g(x)$ - is the outer function
- $h(x)$ is the inner function
- $g'(x)$ is the derivative of $g(x)$
- $h'(x)$ is the derivative of $h(x)$
- $g'(h(x))$ is the derivative of $g(x)$ evaluated at $h(x)$
- $h'(x)$ is the derivative of $h(x)$
- $g'(h(x))h'(x)$ is the product of the two derivatives

### Derivatives of Common Functions

| Initial      | Derivative          |
| ------------ | ------------------- |
| $\large x$   | $\large 1$          |
| $\large x^2$ | $\large 2x$         |
| $\large x^3$ | $\large 3x^2$       |
| $\large e^x$ | $\large e^x$        |
| $\large a^x$ | $\large a^x \ln(a)$ |

### Logarithmic Derivatives

| Initial            | Derivative                 |
| ------------------ | -------------------------- |
| $\large \ln(x)$    | $\large \frac{1}{x}$       |
| $\large \log_a(x)$ | $\large \frac{1}{x\ln(a)}$ |
| $\large \log_a(x)$ | $\large \frac{1}{x\ln(a)}$ |

### Trigonometric Derivatives

| Initial          | Derivative               |
| ---------------- | ------------------------ |
| $\large \sin(x)$ | $\large \cos(x)$         |
| $\large \cos(x)$ | $\large -\sin(x)$        |
| $\large \tan(x)$ | $\large \sec^2(x)$       |
| $\large \cot(x)$ | $\large -\csc^2(x)$      |
| $\large \sec(x)$ | $\large \sec(x)\tan(x)$  |
| $\large \csc(x)$ | $\large -\csc(x)\cot(x)$ |
