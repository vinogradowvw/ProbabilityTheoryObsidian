Kolmogorov's probability axioms is a set of rules (axioms) which is expressing how to formalise probability and objects of it.

Let $(\Omega, \mathcal{F}, P)$ be a ***measure space***

Where:
$\Omega$ is a [[Classic definition of probability|Sample Space]]
$\mathcal{F}$ is an **$\sigma - algebra$** (***event space***) (set of subsets of $\Omega$) (set of any events that is measurable or that is needed to be measured):
	1. $\Omega \in \mathcal{F}$
	2. $A \in \mathcal{F} \implies \neg A \in \mathcal{F}$   |    $(\neg A = \Omega  \setminus A)$  $|\implies \oslash \in \mathcal{F}$
	3. $A, B \in \mathcal{F} \implies A \cup B \in \mathcal{F}, A \cap B\in \mathcal{F}$
$P$ is a measure of probability ($P:\mathcal{F} \to [0,1]$):
	1. $P(\Omega) = 1$
	2. $P(\neg A) = 1- P(A)$
	3. $A, B \in \mathcal{F}, A \cap B = \oslash \implies P(A \cup B) = P(A) + P(B)$
	3.1 $A_{1}, A_{2}\dots A_{\infty} \in \mathcal{F} \implies P(\cup_{i=1}^{\infty}A) = \sum_{i=1}^{\infty}P(A)$
