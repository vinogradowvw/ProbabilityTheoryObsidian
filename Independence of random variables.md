
### Independence
[[Random variable, cumulative distribution function|random variable]] $\xi , \eta$ are **independent**, if:
$$
\forall x, y \in \mathbb{R}: P(\xi \leq x, \eta \leq y) = P(\xi \leq x)P(\eta \leq y) = F_{\xi}(x)F_{\eta}(y)
$$
This looks like the definition of independent events. The key difference is that the random variable can generate more events, so every event that comes from one random variable and from another should be independent.
#### Independence and [[Expected value|expected value]]
If $\xi , \eta$ - **independent** random variables, then:
$$E[\xi \eta]=E[\xi]E[\eta]$$
Proof:
$\xi: \Omega \to \{ x_{1},x_{2},\dots,x_{k} \}$
$\eta: \Omega \to \{ y_{1},y_{2},\dots,y_{m} \}$
$$
\begin{array}{l}
E[\xi, \eta] = \sum_{i=1}^k\sum_{j=1}^m x_{i}y_{j}P(\xi = x_{i}, \eta =y_{j}) \\
= \sum_{i=1}^k\sum_{j=1}^m x_{i}y_{j}P(\xi = x_{i}) P(\eta =y_{j}) \\
= (\sum_{i=1}^k x_{i}P(\xi = x_{i})) (\sum_{j=1}^m y_{j} P(\eta =y_{j})) \\
=E[\xi]E[\eta]
\end{array}
$$
### Independence and [[Covariance and Correlation|correlation]]
If $\xi , \eta$ are not correlated, then:

$\rho(\xi, \eta) = \frac{cov(\xi, \eta)}{\sqrt{ D[\xi] D[\eta] }} = 0 \implies cov(\xi, \eta)=0 \implies E[\xi \eta] - E[\xi]E[\eta] = 0 \implies E[\xi \eta] = E[\xi]E[\eta]$

It follows that $E[\xi \eta] = E[\xi]E[\eta]$ and $\xi$ and $\eta$ are independent.
So if $\xi$ and $\eta$ are independent they are also not correlated. But the converse is not always true. Two random variables that are not correlated could be still dependent.

$\text{Independence} \implies \rho(\xi, \eta) = 0$
$\rho(\xi, \eta) = 0 \cancel{\implies} \text{Independence}$