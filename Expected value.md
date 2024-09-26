---
aliases:
  - expected value
---
Generally, Expected value expresses the mean ("typical") value from all values that the random variable can take, weighted by the probability of it. 
### Discrete random variable
$X: \Omega = \{ \omega_{1}, \omega_{2}, \omega_{3}\dots\omega_{n} \} \to \{ x_{1}, x_{2}, x_{3}\dots x_{n} \}$
$p_{i} - \text{Probability of } \omega_{i}$
$$E[X] = \sum_{i=1}^n X(\omega_{i})*p_{i} = \sum_{i=1}^nx_{i}P(X=x_{i})$$
$X: \Omega = \{ \omega_{n} \}_{n=1}^\infty \to \{ x_{n} \}_{n=1}^\infty \}$
$p_{i} - \text{Probability of } \omega_{i}$
$$E[X] = \sum_{i=1}^\infty X(\omega_{i})*p_{i} = \sum_{i=1}^\infty y_{i}P(X=x_{i})$$
### Continuous random variable

$X: \Omega \to \mathbb{R}$

$$
E[X] = \int_{-\infty}^\infty xf(x)dx
$$
$f(x)$ is [[Absolutely continuous random variable, Probability density function|PDF]]


### Properties of expected value
1. Linearity of $E[X]$
		$E[X_{1}+X_{2}]=E[X_{1}]+E[X_{2}]$
		$E[c_{1}X_{1} + c_{2}X_{2}] = c_{1}E[X_{1}] + c_{2}E[X_{2}]$
2. Non-multiplicativity
		$E[X_{1}X_{2}]\neq E[X_{1}]E[X_{2}]$
3. $E[g(X)]$ :
		Discrete random variable:
			$E[g(X)]=\sum_{i=1}^ng(x_{i})P(X=x_{i})$
		Continuous random variable:
			$E[g(X)]=\int_{-\infty}^\infty g(x)f(x) dx$
4. $E[c] = c$
5. $E[E[X]]=E[X]$
6. $E[cX] = cE[X]$