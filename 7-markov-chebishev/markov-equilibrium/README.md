# Markov Equilibrium

It says that X probability variable can't be much higher than $E(X)$ with big probability.

$P(X \geq t \times E(X)) \leq {1 \over t}$

It means so:

We have a sales agent, who on average sells 64 products a day. 

$E(X) = 64$

Possibility of him selling more than 250 products a day is:

$P(X \geq t \times E(X)) \leq {1 \over t}$

$t \times E(X) = 250$

$t \times 64 = 250$

$t = {64 \over 250} = 0,256$

So he sells today 250 products event has a maximum probability of 0,256.

> If we want to know what possibility he sells less than an amount, we calculate the max possibility of more or equal with **Markov Equilibrium**, and distract it from 1.
