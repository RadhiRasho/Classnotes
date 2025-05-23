# Math 1700 - Project 1

## Introduction

The project explores the Normal Probability Distribution and acts as a proof/argument of the theory that the area under the curve of the Normal Probability Distribution is equal to 1.

## Normal Probability Distribution

$$
\Large
f(x) = \frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{1}{2}(\frac{x - \mu}{\sigma})^2}
$$

Simplifying the function:

$$
\Large
f(x) = \frac{1}{\sqrt{2\pi}}e^{-\frac{x^2}{2}}, \, as \, \mu = 0 \, and \, \sigma = 1
$$

The function above is called the Normal probability density function with the mean $\large \mu$ and the standard deviation $\large \sigma$. The number $\large \mu$ tells where the distribution is centered, and $\large \sigma$ measures the "scatter" around the mean.

From the theory of probability, it is known that:

$$
\Large
\int_{-\infty}^{\infty} f(x)dx = 1
$$

## Graphical Representation

For this project $\large \mu = 0$ and $\large \sigma = 1$.

### $A)$ Graph of $\large f$. Find the interval on which the $\large f$ is increasing, the interval on which $\large f$ is decreasing, and any extreme values and where they occur

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

However, since we know that $\large f$ has an increasing interval at $\large (-\infty, 0)$ and a decreasing interval at $\large (0, \infty)$, we can conclude that $\large f$ has a local maximum at $\large x = 0$, this would also act as the Absolute Maximum. We can also conclude that there is no local minimum nor is there an Absolute Minimum.

### $B)$ Graph

The graph of $\large f$ is shown below:

![Normal Probability Distribution](https://github.com/RadhiRasho/Classnotes/blob/master/Calc_Two/Project_One/Project_One_Graph.png?raw=true)

Graph of $\large \int_{-n}^{n} f(x)dx$ when $\large n = 1, 2, and \, 3$:

![Graph of the integral](https://github.com/RadhiRasho/Classnotes/blob/master/Calc_Two/Project_One/Project_One_Integral_Graph.png?raw=true)

In the image above you'll see the graph of $\large f$ and the graph of $\large \int_{-n}^{n} f(x)dx$ when $\large n = 1, 2, and \, 3$. As $\large n$ increases, the area under the curve of $\large f$ increases and approaches 1.

### $C)$ Give a convincing argument that $\large \int_{-\infty}^{\infty} f(x)dx = 1$

Information provided (hint):

$$
\Large
0 < f(x) < e^{-\frac{x}{2}} \, for \, x > 1 \, and \, b > 1
$$

$$
\Large
\int_{1}^{\infty} e^{-\frac{x}{2}}dx \rightarrow 0 \, as \, b \rightarrow \infty
$$

From the information provided, we can see that $\large f(x)$ is always less than $\large e^{-\frac{x}{2}}$ for $\large x > 1$. We also know that the integral of $\large e^{-\frac{x}{2}}$ from $\large 1$ to $\large \infty$ approaches 0 as $\large b$ approaches $\large \infty$.

Therefore, we can conclude that the area under the curve of $\large f$ approaches 1 as $\large n$ approaches $\large \infty$, meaning that $\large \int_{-\infty}^{\infty} f(x) dx = 1$.
