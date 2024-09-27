---
aliases:
  - covariance
  - correlation
---

### Covariance
Covariance is a measure of joint variance of two random variables. If high values of $\xi$ are mostly followed with high values of $\eta$  or the same with low values (two variables have same behaviour) - than covariance is positive. If two variables have opposite behaviour - the covariance is negative. If two variable shows just different behaviour - the covariance $\approx 0$.
$$
\begin{array}{}
cov(\xi, \eta) = E[ (\xi - E[\xi]) (\eta - E[\eta])] \\ \\
= E[\xi \eta] - E[\xi]E[\eta]
\end{array}{}
$$
Variance and covariance:
$$
cov(\xi, \xi) = D[\xi]
$$

### Correlation
Correlation measures similarity of behaviours of two random variables. Moreover, the correlation expresses the power of **linear** relationship between two random variables.
$$
\rho(\xi, \eta) = \frac{cov(\xi, \eta)}{\sqrt{ D[\xi] D[\eta] }} \in [-1;1]
$$

#### Correlation and [[Variance]]
If $\xi , \eta$ are not correlated, then:
$$
D[\xi+\eta] = D[\xi] + D[\eta]
$$
Proof:
$$
\begin{array}{l}
D[\xi + \eta] = E[(\xi + \eta)^2] - E[\xi+\eta]^2 \\
= E[\xi^2 + 2\xi \eta +\eta^2] - E[\xi]^2 -E[\xi]^2 - 2E[\xi]E[\eta] - E[\eta]^2 \\
= E[\xi^2] + 2E[\xi \eta] + E[\eta^2] -E[\xi]^2 -2E[\xi]E[\eta] - E[\eta]^2 \\ \\
 & \rho = 0 \implies E[\xi \eta] = E[\xi] E[\eta] \\
= E[\xi]^2 + \cancel{2E[\xi]E[\eta]} + E[\eta^2] -E[\xi]^2 - \cancel{2E[\xi]E[\eta]} -E[\eta]^2 \\
= (E[\xi]^2  -E[\xi]^2) + (E[\eta^2] -E[\eta]^2) \\
 & E[\xi^2] - E[\xi]^2 = D[\xi] \\
 & E[\eta^2] - E[\eta]^2 = D[\eta] \\
= D[\xi] + D[\eta]
\end{array}{}
$$

