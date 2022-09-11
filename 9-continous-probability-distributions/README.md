# Continous Probability Distributions

Distributions of continous probability variables. Generally they are for times, or continous quantities, like liters, kilogramms, smth. Stuff, where $P(X=a) = 0$, where we can only ask intervals, like $P(X < a)$, $P(X > a)$, $P(a < X < b)$

> $P(X=a) = 0$ means, that if we order a 0,5l beer, we will either get a little more, or a little less. Never exactly 0,5000000l

We have the following distributions, and their basic functions:

![Continous Probability Distribution 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_1.png)

To get $P$-s, we can do the following:

![Continous Probability Distribution 2](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_2.png)

### Uniform Distribution:

We are waiting a phone call. (yay! 😱) Call will come between 2p.m. and 7p.m., all times with the same possibility. What is the possibility, that we will get it before 4p.m.?

> X = what is the time

$P(X < 4) = ?$

$P(X < 4) = F(4) = \cases{0|x ≤ A|\frac{x-A|B-A}|A < x ≤ B|1|B < x} = \cases{0|x ≤ 2|\frac{x-2|7-2}|2 < x ≤ 7|1|7< x} = \frac{4-2|7-2} = \frac{2|5} = 0,4$