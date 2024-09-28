## Markov's inequality
Provides an upper bound for probability of non-negative random variable is greater or equal to some $a$.
$\xi : \Omega \to \{ x_{1},x_{2},x_{3}\dots x_{k} \}, \forall i: x_{i} \geq 0$
$$
\forall a , a> 0: P(\xi \geq a) \leq \frac{E[\xi]}{a}
$$
Proof:
$$
\begin{array}{l}
E[\xi] = \sum_{i=1}^k x_{i}P(\xi = x_{i}) \\
= \sum_{i:x_{i}\geq a} x_{i}P(\xi = x_{i}) + \sum_{i:x_{i} < a} x_{i}P(\xi = x_{i}) \\ \\

\sum_{i:x_{i} < a} x_{i}P(\xi = x_{i}) \geq 0 \\
\sum_{i:x_{i}\geq a} x_{i}P(\xi = x_{i}) \geq a\sum_{i:x_{i}\geq a}P(\xi = x_{i}) = a P(\xi \geq a) \\
E[\xi] \geq a P(\xi \geq a) \\
P(\xi \geq a) \leq \frac{E[\xi]}{a}
\end{array}{}
$$

## Chebyshev's inequality
Refers to [[#Markov's inequality]].
Provides an upper bound for the probability that the difference between any random variable with finite variance and its expectation (deviation) is greater than some positive constant $a$
$$
\forall \xi, D[\xi] < \infty ; \forall a, a>0 : P(\xi - E[\xi] \geq a) \leq \frac{D[\xi]}{a^2}
$$
Proof:
$$
\begin{array}{l}
\eta := (\xi-E[\xi])^2   \\
\text{From Markov's inequality : }P(\eta \geq a^2) \leq \frac{E[\eta]}{a^2} \\
E[\eta] = E[(\xi-E[\xi])^2] = D[\xi] \\
 \\
P(\eta \geq a^2) \leq \frac{D[\xi]}{a^2} \\
P((\xi-E[\xi])^2  \geq a^2)  \leq \frac{D[\xi]}{a^2}  \\ \\

\implies P((\xi-E[\xi]) \geq a)\leq \frac{D[\xi]}{a^2} 
\end{array}
$$
