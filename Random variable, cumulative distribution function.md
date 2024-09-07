---
aliases:
  - random variable
  - cumulative distribution function
  - CDF
---
# Random variable
Random variable is a mathematical formalization of a measurable property of an random object from [[Classic definition of probability|Sample Space]] $\Omega$

Formally:

(Operating on $(\Omega, \mathcal{F}, P)$ from [[Kolmogorov's probability axioms]])

A random variable $\xi$ is a measurable function that operates on sample space $\Omega$:
	$\xi : \Omega \to \mathbb{R}$

The word measurable means that:
	$\forall x \in \mathbb{R}: \{ \omega \in \Omega: \xi(\omega) \leq x \} \in \mathcal{F}$
That means that it is possible to measure a probability of $\xi(\omega)$ being less than any $x \in \mathbb{R}$. So here, $\{\omega \in \Omega: \xi(\omega) \leq x\}$  is an event from $\mathcal{F}$.

$\implies$
$$
P(\xi\leq x) = P(\{\omega \in \Omega: \xi(\omega) \leq x\})
$$
If it is possible to calculate this probability, from the properties of the [[Kolmogorov's probability axioms]] it follows that it is possible to calculate other probabilities such as: $P(\xi>x)$ or for any $B \subset \mathbb{R}: P(\xi\in B)$.

# Cumulative distribution function

Cumulative distribution function of a [[Random variable, cumulative distribution function|random variable]] $\xi$ evaluated at x is the probability that $\xi$ will take a value less or equal to x.

$$
F_{\xi}(x) = P(\xi \leq x)
$$
Properties of CDF:
1. $F_{\xi} (x) \in [0,1]$
2. $F_{\xi}$ is a monotonically non-decreasing function
3. $F_{\xi}$ is a right-continuous function.
4. $\lim_{ x \to \infty }F_{\xi}(x) = 1$
5. $\lim_{ x \to - \infty }F_{\xi} =0$

![[cdf-normal.png]]
![[cdf-discrete.png]]