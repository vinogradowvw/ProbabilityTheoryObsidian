
The poisson limit theorem states that in some conditions, it is possible to approximate the binomial distribution.

Given set of $n$ experiments in the [[Bernoulli scheme]] with $p_{n}$ probability of "success" and $\mu_{n}$ number of "success" events.

Then if:
	$\lim_{ n \to \infty }np_{n} = \lambda$, $\lambda > 0$
In other words:
	$np_{n}\sim \lambda$;
	$p_{n} \sim \frac{\lambda}{n}$

$$
P(\mu_{n}=k) \sim \frac{{\lambda^k e^{-\lambda}}}{k!}
$$
Or:
$$
\lim_{ n \to \infty } P(\mu_{n}=k) = \frac{{\lambda^k e^{-\lambda}}}{k!}
$$

Proof:
$C_{n}^{k}p^{k}q^{n-k} \sim \frac{n!}{k!(n-k)!}\cdot \frac{\lambda}{n}^k\cdot\left( 1-(1+o(1))\frac{\lambda}{n} \right)^{n-k}$
	$\sim \frac{{n(n-1)(n-2)\dots 2\cdot 1}}{k!\cdot ((n-k)(n-k-1)\dots 2\cdot 1)} \cdot \frac{\lambda}{n}^k\cdot( 1-(1+o(1))\frac{\lambda}{n} )^{n-k}$
	$\sim  \frac{{n(n-1)(n-2)\dots (n-k+1)}}{k!} \cdot \frac{\lambda}{n}^k\cdot( 1-(1+o(1))\frac{\lambda}{n})^{n-k}$
	$\sim \frac{n^k}{k!}\cdot \frac{\lambda^k}{n^k}\cdot\left( 1-(1+o(1))\frac{\lambda}{n} \right)^{n-k}$
			$( 1-(1+o(1))\frac{\lambda}{n})^{n-k} =( 1-(1+o(1))\frac{\lambda}{n})^{n}\cdot( 1-(1+o(1))\frac{\lambda}{n})^{-k}$ 
			*1)* $(1-(1+o(1))\frac{\lambda}{n})^{-k} \sim 1$
			*2)* $(1-(1+o(1))\frac{\lambda}{n})^{n} \sim e^{-\lambda}$
	$\sim \frac{n^k}{k!}\cdot \frac{\lambda^k}{n^k} \cdot e^{-\lambda}$
	$\sim \frac{\lambda^{k}e^{-\lambda}}{k!}$

