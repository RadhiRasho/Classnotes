# Math 1700 - Project 1

## Introduction

The project explores the Normal Probability Distribution and acts as a proof/argument of the theory that the area under the curve of the Normal Probability Distribution is equal to 1.

## Normal Probability Distribution

$$
\Large
f(x) = \frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{(x - \mu)^2}{2\sigma^2}}
$$

The function above is called the Normal probability density function with the mean $\large \mu$ and the standard deviation $\large \sigma$. The number $\large \mu$ tells where the distribution is centered, and $\large \sigma$ measures the "scatter" around the mean.

From the theory of probability, it is known that:

$$
\Large
\int_{-\infty}^{\infty} f(x)dx = 1
$$

## Graphical Representation

For this project $\large \mu = 0$ and $\large \sigma = 1$.

### $A)$ Graph of $\large f$. Find the interval on which the $\large f$ is increasing, the interval on which $\large f$ is decreasing, and any extreme values and where they occur.

To determin the intervals on which $\large f$ is increasing and decreasing, we need to find the derivative of $\large f$.

$$
\Large
f'(x) = \frac{d}{dx} \left( \frac{1}{\sqrt{2\pi}}e^{-\frac{x^2}{2}} \right)
$$

$$
\Large
f'(x) = \frac{d}{dx} \left( \frac{1}{\sqrt{2\pi}} \right) e^{-\frac{x^2}{2}} + \frac{1}{\sqrt{2\pi}} \frac{d}{dx} \left( e^{-\frac{x^2}{2}} \right) = -\frac{x}{\sqrt{2\pi}} e^{-\frac{1}{2}x^2}
$$

To find the critical points, we need to solve the equation $\large f'(x) = 0$. 

$$
\Large
-\frac{x}{\sqrt{2\pi}} e^{-\frac{1}{2}x^2} = 0
$$

$$
\Large
x = 0
$$

The critical point is at $\large x = 0$. To determine the intervals on which $\large f$ is increasing and decreasing, we need to find the sign of $\large f'(x)$.

$$
\Large
f'(x) = -\frac{x}{\sqrt{2\pi}} e^{-\frac{1}{2}x^2}
$$

$$
\Large
f'(x) = \begin{cases}
      > 0 & x < 0 \\
      < 0 & x > 0
   \end{cases}
$$

Therefore, $\large f$ is increasing on the interval $\large (-\infty, 0)$ and decreasing on the interval $\large (0, \infty)$.

### Finding Local Maximums and Minimums

Typically you'd go on to find the second derivative of $\large f$ and use the second derivative test to find the local maximums and minimums. 

However, since we know that the has a increasing interval at $\large (-\infty, 0)$ and a decreasing interval at $\large (0, \infty)$, we can conclude that $\large f$ has a local maximum at $\large x = 0$, this would also act as the Absolute Maximum. We can also conclude that there is no local minimum nor is there an Absolute Minimum.