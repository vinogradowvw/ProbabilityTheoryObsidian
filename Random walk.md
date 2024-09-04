Basic form of random walk is one-dimensional random walk.
This is stochastic process on integer line, $\mathbb{Z}$, which starts on 0 and each at each steps moves forward (+1) or backwards (-1).

![[random-walk.png]]

The basic problem here is to find a probability of ending on position of $k \in \mathbb{Z}$ after n steps (event $A$).

Solution:
$x$ = number of steps forward;
$n-x$ = number of steps backwards;

Given that the process starts on 0:
$k = 0 + x - (n - x) = 2x - n$      *($k$ - final position)*
$x = \frac{{k+n}}{2}$
Here $k+n$ must be even, otherwise **probability = 0**.
$$
P(A) = C_{n}^{x} \cdot p^x \cdot p^{n-x}
$$
Random walk can be viewed as a realization of [[Bernoulli scheme]], where each trial corresponds to one step in the random walk, and the overall path of the walk is determined by the sum of the results of these trials.