---
aliases:
  - absolutely continuous random variable
  - continuous random variable
  - probability density function
  - density
  - PDF
---

The **absolutely continuous random variable** is a [[Random variable, cumulative distribution function|random variable]] which has an absolutely continuous probability distribution. The sample space is usually $\Omega = \mathbb{R}$.

The probability of absolutely continuous random variable is described by **probability density function $f(x)$.**
$$
P(a\leq X\leq b) = \int_{a}^b f{(x)} dx
$$
It follows:

$$
\int_{-\infty}^\infty f(x)dx = 1
$$

Probability for X to take a single value is always 0:
$$P(X=a) = P(a\leq X \leq a) = 0$$
[[Random variable, cumulative distribution function|CDF]]:
$$
F(x) = P(X\leq x) = \int_{-\infty}^x f(x) dx
$$