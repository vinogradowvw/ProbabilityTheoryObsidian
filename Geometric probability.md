---
id: Geometric probability
aliases: []
tags: []
---
Geometric probability is a tool to solve probability problems with infinite amounts of outcomes. Those problems involve continuous variables (such as time).

# Basic geometric probability problem
"Two persons agreed to meet between 9:00 and 10:00. Each person will come in random moment in this interval and wait for 15 minutes. We need to find a probability of meet."

From the fact that time is continuous variable it is impossible to count all possible outcomes and apply a  [[Classic definition of probability]] to solve this problem.

In this problem the set of all outcomes when those persons will meet is just a set of points $|A-B| \leq 0.25$ 

The condition $∣A−B∣≤0.25$ represents the requirement that the absolute difference between the arrival times of the two persons must be less than or equal to 15 minutes (0.25 hours) for them to meet.
![[geometric-probability.png]]
Here, on the plot the point represents a single outcome.
The set of points that represent the event when those persons will meet is between this line.

$\Omega = [0, 1]^2$

To find the probability of this event happening we need to divide the area (Peano–Jordan measure) between lines by the total area.

$$
P = \frac{\frac{7}{16}}{1} = \frac{7}{16}
$$

Here, the property of probability $P(A) = 1 \Leftrightarrow A = \Omega$ is not applicable, thus the probability of a single outcome here equals zero, because the measure of a point equals zero. So if we will take out a single point from $A$ the probability $P(A) = 1$ , but $A \neq \Omega$.
For geometric probability we can substitute this property by $P(A) = 1 \Leftarrow A = \Omega$
