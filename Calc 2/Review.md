# Day 1: Calculus $\Iota$ Review

## Derivative Rules for Basic Functions

### Power Rule For Derivatives

$$
\large
\frac{d}{dx} x^n = nx^{n-1}
$$

### Constant Rule For Derivatives

$$
\large
\frac{d}{dx} C = 0, \nobreakspace C = \text{any constant}
$$

### Sum Rule For Derivatives

$$
\large
\frac{d}{dx} f(x) + g(x) = f'(x) + g'(x)
$$

### Product Rule For Derivatives

$$
\large
\frac{d}{dx} (f(x)g(x)) = f'(x)g(x) + f(x)g'(x)
$$

### Quotient Rule For Derivatives

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

### Chain Rule For Derivatives

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

## Integrals

### Indefinite Integrals

An indefinite integral is a function that represents the anti-derivative of another function. It is used to find the general form of the anti-derivative of a function.

The indefinite integral of a function $\large f(x)$ is denoted by $\large \int f(x) \, dx$.

### Definite Integrals

A definite integral is a number that represents the signed area under the curve of a function between two points. It is used to find the exact area under the curve of a function over a given interval.

The definite integral of a function $\large f(x)$ from $\large a$ to $\large b$ is denoted by $\large \int_{a}^{b} f(x) \, dx$.

## Integration Rules for Basic Functions

### Power Rule for Integration

$$
\large
\int x^n \, dx = \frac{x^{n+1}}{n+1} + C, \nobreakspace n \neq -1
$$

### Constant Rule for Integration

$$
\large
\int C \, dx = Cx + C, \nobreakspace C = \text{any constant}
$$

## Integration Rules for Area of Solids

### Area Between Two Curves

The area between two curves is the region enclosed by the graphs of two functions. To find the area between two curves, you need to determine the points of intersection and integrate the difference between the two functions over the interval.

The area between two curves $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ is given by:

$$
\LARGE
\int_{a}^{b} [f(x) - g(x)] \, dx
$$

### Volume of Revolution

The volume of revolution is the volume of a solid formed by rotating a region enclosed by two functions around a given axis. To find the volume of revolution, you need to determine the points of intersection and integrate the area of the cross-sections over the interval.

The volume of revolution of a region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ rotated around the $\large x$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(x)^2 - g(x)^2] \, dx
$$

The volume of revolution of a region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ rotated around the $\large y$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(y)^2 - g(y)^2] \, dy
$$

### Arc Length

The arc length is the length of a curve between two points. To find the arc length, you need to integrate the square root of the sum of the squares of the derivatives of the functions over the interval.

The arc length of a curve $\large f(x)$ from $\large a$ to $\large b$ is given by:

$$
\LARGE
\int_{a}^{b} \sqrt{1 + [f'(x)]^2} \, dx
$$

### Surface Area of Revolution

The surface area of revolution is the surface area of a solid formed by rotating a curve around a given axis. To find the surface area of revolution, you need to integrate the arc length of the curve over the interval.

The surface area of revolution of a curve $\large f(x)$ from $\large a$ to $\large b$ rotated around the $\large x$-axis is given by:

$$
\LARGE
2\pi \int_{a}^{b} f(x) \sqrt{1 + [f'(x)]^2} \, dx
$$

The surface area of revolution of a curve $\large f(x)$ from $\large a$ to $\large b$ rotated around the $\large y$-axis is given by:

$$
\LARGE
2\pi \int_{a}^{b} x \sqrt{1 + [f'(x)]^2} \, dx
$$

### Triangle Area of Revolution

The triangle area of revolution is the area of a solid formed by rotating a triangle around a given axis. To find the triangle area of revolution, you need to integrate the area of the cross-sections over the interval.

The triangle area of revolution of a triangle with base $\large b$ and height $\large h$ rotated around the $\large x$-axis is given by:

$$
\LARGE
\frac{1}{2} \pi \int_{a}^{b} [f(x)]^2 \, dx
$$

The triangle area of revolution of a triangle with base $\large b$ and height $\large h$ rotated around the $\large y$-axis is given by:
****
$$
\LARGE
\frac{1}{2} \pi \int_{a}^{b} [f(y)]^2 \, dy
$$

### Solid generated by revolving the region bounded by graph

The solid generated by revolving the region bounded by the graph of a function around the $\large x$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(x)]^2 \, dx
$$

The solid generated by revolving the region bounded by the graph of a function around the $\large y$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(y)]^2 \, dy
$$

### Solid generated by revolving the region bounded by the parabola

The solid generated by revolving the region bounded by the parabola $\large y = x^2$ around the $\large x$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [x^2]^2 \, dx
$$

The solid generated by revolving the region bounded by the parabola $\large y = x^2$ around the $\large y$-axis is given by:

$$
\LARGE
\pi \int_{a}^{b} [y^2]^2 \, dy
$$

### Shell Method

The shell method is used to find the volume of a solid formed by rotating a region enclosed by two functions around a given axis. To find the volume using the shell method, you need to integrate the circumference of the shell times the height of the shell over the interval.

The volume of a solid generated by revolving the region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ around the $\large y$-axis using the shell method is given by:

$$
\LARGE
2\pi \int_{a}^{b} x[f(x) - g(x)] \, dx
$$

The volume of a solid generated by revolving the region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ around the $\large x$-axis using the shell method is given by:

$$
\LARGE
2\pi \int_{a}^{b} y[f(y) - g(y)] \, dy
$$

### Washer Method

The washer method is used to find the volume of a solid formed by rotating a region enclosed by two functions around a given axis. To find the volume using the washer method, you need to integrate the difference between the outer and inner radii squared times $\large \pi$ over the interval.

The volume of a solid generated by revolving the region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ around the $\large y$-axis using the washer method is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(x)^2 - g(x)^2] \, dx
$$

The volume of a solid generated by revolving the region between $\large f(x)$ and $\large g(x)$ from $\large a$ to $\large b$ around the $\large x$-axis using the washer method is given by:

$$
\LARGE
\pi \int_{a}^{b} [f(y)^2 - g(y)^2] \, dy
$$
