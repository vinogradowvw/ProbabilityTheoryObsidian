The Binomial Distribution represents the [[Random variable, cumulative distribution function|distribution]] of the number $\mu_{n}$ of "success" events with probability $p$ in $n$ experiments ([[Bernoulli scheme]]).

From the [[Bernoulli scheme]] definitions:
	$\omega = (x_{1}, x_{2}, x_{3}\dots x_{n})$; 
	$x_{i} = 0$ if failure, $x_{i} = 1$ if success
It follows:
	$\mu_{n} (\omega) = \sum_{i=1}^n x_{i}$

In context of binomial **distribution**, $\mu_{n}$ is binomial [[Random variable, cumulative distribution function|random variable]] with binomial distribution.
$$\mu_{n} \sim Binom(n, p)$$

The [[PMF]] of the Binomial Distribution is given by:
$$
P(\mu_{n} = x) = {C}_{n}^x \cdot p^x \cdot q^{n-x}
$$
And the [[Random variable, cumulative distribution function|CDF]] of Binomial Distribution is:
$$
P(\mu_{n} \leq x) =  \sum_{k\leq x} P(\mu = k) 
$$
![[binompmf.png]]
![[binomcdf.png]] 