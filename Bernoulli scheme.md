There are n experiments, in each can occur certain event (that is counts as success) with probability $p$, and opposite event ("failure") with probability $q=1-p$. The problem is to find a probability of exactly m "success" events happening in n experiments.

$p \in [0, 1]$
$q = 1-p \in [0, 1]$
$n =$ number of experiments

In Bernoulli scheme an [[Classic definition of probability|Outcome]] is a sequence of results (events - success or failure) of n experiments. All events must be independent.

$\omega = (x_{1}, x_{2}, x_{3}\dots x_{n})$; 
$x_{i} = 0$ if failure, $x_{i} = 1$ if success

[[Classic definition of probability|Sample Space]]
$\Omega = 2^n$

Then the probability of an outcome equals:
$$P(\omega) = p^{\sum_{i=0}^{n}x_{i}} \cdot q^{n-\sum_{i=0}^{n}x_{i}}$$

And an [[Classic definition of probability|Event]] $A$ ( in $n$ experiments there is $k$ "success" events and $n-k$ "failure" events ), $A \subset \Omega$ has probability:
$$
P(A) = {C}_{n}^k \cdot p^k \cdot q^{n-k}
$$
