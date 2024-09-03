---
aliases:
  - conditional probability
  - independent
  - mutually independent
  - total probability
---
# Definition of Conditional probability

Given:
	[[Classic definition of probability|Sample Space]] $\Omega$ 
	[[Classic definition of probability|Event]] $A, A \supset \Omega$
	[[Classic definition of probability|Event]] $B, B \supset \Omega$
Probability of $A$ given that $B$ is already known to have occurred.
$\Omega = {\omega_{1}, \omega_{2}, \omega_{3}\dots, \omega_{n}}$
$P(A|B) = \frac{\frac{\frac{|A\cap B|}{|\omega|}}{|B|}}{|\omega|}$
$P(A|B) = \frac{P(A\cap B)}{P(B)}$

From this equation,
$P(A\cap B) = P(A|B)P(B)$

# Independence

Two events are **independent** if:

$P(A\cap B) = P(A) \cdot P(B)$
$P(A|B)  = P(A)$
$P(B|A) = P(B)$

The set of events ${A_{1}, A_{2}, A_{3} \dots A_{n}}$ are **mutually independent** if the probability of every possible subset of events is multiplication of probabilities of those events:
$$
\forall I \subset {1,2, \dots n} : P(\cap_{i \in I } A_{i}) = \prod\limits_{i \in I}P(A_{i})
$$
# Law of total probability
![[law-of-total-probability.png]]
Given:
	$({B_{1},B_{2},B_{3}\dots B_{n} }) = \Omega$ ($\Omega$ is divided into a lot of $B$)
	$\forall B : P(B) \neq 0$
	Random event $A, A \supset \Omega$

$P(A)  = \sum_{n=1}^{\infty}P(A\cap B_{i})_\cdot = \sum_{i=1}^{n}P(A|B_{i}) \cdot P(B_{i})$

This law expresses the total probability of an outcome which can be realized via several distinct events. The formula expresses how to find a probability of event $A$ from the conditional probabilities of $A$ happening with events $B_{i}$.
# Bayes' formula
The [[#Law of total probability]] shows how to find a probability of event $A$ from the conditional probabilities of $A$ happening with events $B_{i}$

The bayes' formula has reverse principle. It aims to find a conditional probability of event $B_{i}$ happening if event $A$ have occurred $P(B_{i}|A)$

From [[#Definition of Conditional probability]] : 
$P(A \cap B) = P(A|B) \cdot P(B) = P(B|A) \cdot P(A)$

From those equations and [[#Law of total probability]] :
$$
P(B_{i}|A) = \frac{P(A | B_{i}) \cdot P(B_{i})}{P(A)} = \frac{P(A | B_{i}) \cdot P(B_{i})}{\sum_{j=1}^{n}P(A|B_{j}) \cdot P(B_{j})}
$$