# Math 1700 - Project 2

## Introduction

This project explores the use of Series in safe and effective dosage of drugs calculations. When a single dose of drug is administered, the drug concentration in the bloodstream can be modeled as a series. The dosage is lost slowly over time, and the concentration can be modeled as a series of decreasing terms.

## Model for Effect of Repeated Doses

$$
\LARGE
 R_n = C_0e^{-kt_0} + C_0e^{-2kt_0} + \ldots + C_0e^{-nkt_0}
$$

Where:

- $\large C_0$ is the change in concentration achievable by a single dose (mg/mL)
- $\large k$ is the elimination constant ($h^{-1}$)
- $\large t_0$ is the time between doses ( $h$ )

The graph below shows the concentration of the drug in the bloodstream over time. The x-axis represents time in hours, and the y-axis represents the concentration of the drug in mg/mL. The graph shows how the concentration of the drug decreases over time after each dose.

![Concentration VS Time Graph](https://github.com/RadhiRasho/Classnotes/blob/master/Calc_Two/Project_Two/Project_Two_Concentration_VS_Time_Graph.png?raw=true)

## Questions to Answer

### $A)$ Write $R_n$ in closed form as single fraction, and find $R = \lim_{n \to \infty} R_n$

The given expression for $R_n$ is:

$$
\Large
 R_n = C_0e^{-kt_0} + C_0e^{-2kt_0} + \ldots + C_0e^{-nkt_0}
$$

This expression can be simplified using by taking the common factor $C_0$ out of the summation:
$$
\Large
 R_n = C_0 \left( e^{-kt_0} + e^{-2kt_0} + \ldots + e^{-nkt_0} \right)
$$

For simplicity, let $x = e^{-kt_0}$. Then we can rewrite the expression as:
$$
\Large
 R_n = C_0 \left( x + x^2 + \ldots + x^n \right)
$$

The terms in the parentheses form a geometric series with first term $\large x$ and common ratio (i.e. $\large r$) $\large x$.

The sum of a geometric series can be calculated using the formula:
$$
\Large
 S_n = \frac{a(1 - r^n)}{1 - r}
$$
Where:

- $\large a = x = e^{-kt_0}$ is the first term
- $\large r = x = e^{-kt_0}$ is the common ratio
- $\large n$ is the number of terms.

From here, we can start substituting our values into the formula:

$$
\Large
 R_n = C_0 \left( \frac{x(1 - x^n)}{1 - x} \right)
$$

Now, substituting back for $x$:
$$
\Large
 R_n = C_0 \left( \frac{e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}} \right)
$$

Or you can write it as a single fraction:
$$
\Large
 R_n = \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}}
$$

That is the closed form of $\large R_n$.

Now, we need to find the limit of $\large R_n$ as $\large n \to \infty$:
$$
\Large
 R = \lim_{n \to \infty} R_n = \lim_{n \to \infty} \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}}
$$

Sense $\large k > 0$ and $\large t_0 > 0$, the term $\large e^{-kt_0}$ is a positive number. Meaning it will be in the following interval: $\large 0 < e^{-kt_0} < 1$.

As $\large n \to \infty$, the term $\large e^{-nkt_0} \to 0$, because it's a number between 0 and 1 raised to a large positive power, meaning it gets smaller the larger $\large n$ becomes.

Therefore, we can conclude that:
$$
\Large
 \lim_{n \to \infty} e^{-nkt_0} = 0
$$

Sense we've established that, we can now substitute it into our limit:
$$
\Large
 R = \frac{C_0 e^{-kt_0}(1 - 0)}{1 - e^{-kt_0}}
$$

$$
\Large
 R = \frac{C_0 e^{-kt_0}}{1 - e^{-kt_0}}
$$

In this case, $\large R$ represents the total concentration of the drug in the bloodstream after many doses.

### $B)$ Calculate $R_1$ and $R_10$ for $C_0 = 1(mg/mL)$, $k = 0.1h^{-1}$, and $t_0 = 10h$. How good an estimate of $R$ is $R_10$?

What we are given:

- $\large C_0 = 1(mg/mL)$
- $\large k = 0.1h^{-1}$
- $\large t_0 = 10h$

We can simplify some of our solving for some of the variables:

- $\large -kt_0 = -0.1(10) = -1$
- $\large e^{-kt_0} = e^{-1} \approx 0.36788$

To calculate $\large R_1$, we can use the fact that $\large R_1$ is just the first term of the series:
$$
\Large
 R_1 = C_0 e^{-kt_0} = 1 \cdot e^{-1} \approx 0.36788 \, (mg/mL)
$$

We could have also just used the closed form of $\large R_n$ to calculate $\large R_1$:
$$
\Large
 R_1 = \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}} = \frac{1 \cdot e^{-1}(1 - e^{-1})}{1 - e^{-1}} = 0.36788 \, (mg/mL)
$$

This shows that the closed form of $\large R_n$ is correct.

To calculate $\large R_{10}$, we can use the closed form of $\large R_n$:
$$
\Large
 R_{10} = \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}}
$$

$$
\Large
    R_{10} = \frac{1 \cdot e^{-1}(1 - e^{-10})}{1 - e^{-1}}
$$

$$
\Large
    R_{10} = \frac{1 \cdot 0.36788(1 - 0.0000454)}{1 - 0.36788}
$$

$$
\Large
    R_{10} = \frac{ 0.36788 \cdot 0.99995}{0.63212} \approx 0.58195 \, (mg/mL)
$$

Therefore, $\large R_{10} \approx 0.58195 \, (mg/mL)$.

This is a good estimate of $\large R$, because the difference between $\large R$ and $\large R_{10}$ is small.

To check the difference between $\large R$ and $\large R_{10}$, we can calculate $\large R$ using the $R$ formula we derived in part A:

$$
\Large
 R = \frac{C_0 e^{-kt_0}}{1 - e^{-kt_0}} = \frac{1 \cdot e^{-1}}{1 - e^{-1}} = \frac{0.36788}{1 - 0.36788}
$$

$$
\Large
 R = \frac{0.36788}{0.63212} \approx 0.58198 \, (mg/mL)
$$

The difference between $\large R$ and $\large R_{10}$ is:
$$
\Large
 R - R_{10} = 0.58198 - 0.58195 \approx 0.00003 \, (mg/mL)
$$

This is a very small difference, which shows that $\large R_{10}$ is a good estimate of $\large R$.

Percentage difference is calculated as:
$$
\Large
 \frac{R - R_{10}}{R} \cdot 100 = \frac{0.58198 - 0.58195}{0.58198} \cdot 100 \approx 0.0052\%
$$

#### Conclusion

Using the calculations above, I was able to conclude that the difference between $\large R$ and $\large R_{10}$ is very small, which means that $\large R_{10}$ is an extremely good estimate of $\large R$. Meaning that after 10 doses, the concentration of the drug in the bloodstream is very close to the long-term concentration/steady state value.

### $C)$ If $k = 0.01h^{-1}$, $t_0 = 10h$, find the smallest n such that $R_n > (\frac{1}{2})R$. Use $C_0 = 1(mg/mL)$

What we are given:

- $\large C_0 = 1(mg/mL)$
- $\large k = 0.01h^{-1}$
- $\large t_0 = 10h$

We can simplify some of our solving for some of the variables:

- $\large -kt_0 = -0.01(10) = -0.1$
- $\large e^{-kt_0} = e^{-0.1} \approx 0.90484$

We can now use this to calculate $\large R$:
$$
\Large
 R = \frac{C_0 e^{-kt_0}}{1 - e^{-kt_0}}
$$

$$
\Large
 R = \frac{1 \cdot e^{-0.1}}{1 - e^{-0.1}}
$$

$$
\Large
 R = \frac{0.90484}{1 - 0.90484}
$$
$$
\Large
 R = \frac{0.90484}{0.09516}
$$
$$
\Large
 R = 9.5083 \,(mg/mL)
$$

$$
\Large
 \frac{1}{2}R = \frac{9.5083}{2} \approx 4.75415 \,(mg/mL)
$$

The inequality we need to solve is:

$$
\Large
 R_n = \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}} > \frac{1}{2}R
$$

$$
\Large
 \frac{C_0 e^{-kt_0}(1 - e^{-nkt_0})}{1 - e^{-kt_0}} > \frac{9.5083}{2}
$$

To solve this inequality, we can start by substituting in the values we know:

$$
\Large
 \frac{1 \cdot e^{-0.1}(1 - e^{-n(0.01)(10)})}{1 - e^{-0.1}} > 4.75415
$$
$$
\Large
 \frac{e^{-0.1}(1 - e^{-0.1n})}{1 - e^{-0.1}} > 4.75415
$$
$$
\Large
 \frac{0.90484(1 - e^{-0.1n})}{0.09516} > 4.75415
$$

Multiply both sides by $\large 0.09516$ to eliminate the fraction:

$$
\Large
 0.90484(1 - e^{-0.1n}) > 4.75415 \cdot 0.09516
$$
$$
\Large
 0.90484(1 - e^{-0.1n}) > 0.4514
$$

Now, divide both sides by $\large 0.90484$ to isolate the term with $\large n$:

$$
\Large
 1 - e^{-0.1n} > \frac{0.4514}{0.90484}
$$
$$
\Large
 1 - e^{-0.1n} > 0.4984
$$

Now, we can isolate the term with $\large n$:

$$
\Large
 - e^{-0.1n} > 0.4984 - 1
$$
$$
\Large
 - e^{-0.1n} > -0.5016
$$
$$
\Large
 e^{-0.1n} < 0.5016
$$

Now, we can take the natural logarithm of both sides to solve for $\large n$:

$$
\Large
 \ln(e^{-0.1n}) < \ln(0.5016)
$$
Now, we can divide both sides by $\large -0.1$:

$$
\Large
 -0.1n < \ln(0.5016)
$$

$$
\Large
 n > \frac{\ln(0.5016)}{-0.1}
$$

$$
\Large
 n > \frac{-0.6931}{-0.1}
$$

$$
\Large
 n > 6.931
$$

Since $\large n$ must be a whole number, we can round up to the next whole number:
$$
\Large
 n = 6.931 \approx 7
$$

Therefore, the smallest $\large n$ such that $\large R_n > \frac{1}{2}R$ is $\large n = 7$. This means that after 8 doses ($\large n=7$ corresponds to the concentration before does $\large n+1=8$), the concentration of the drug in the bloodstream will be greater than half of the long-term concentration/steady state value.
