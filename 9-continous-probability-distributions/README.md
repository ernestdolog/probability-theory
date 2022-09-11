# Continous Probability Distributions

Distributions of continous probability variables. Generally they are for times, or continous quantities, like liters, kilogramms, smth. Stuff, where $P(X=a) = 0$, where we can only ask intervals, like $P(X < a)$, $P(X > a)$, $P(a < X < b)$

> $P(X=a) = 0$ means, that if we order a 0,5l beer, we will either get a little more, or a little less. Never exactly 0,5000000l

We have the following distributions, and their basic functions:

![Continous Probability Distribution 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_1.png)

To get $P$-s, we can do the following:

![Continous Probability Distribution 2](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_2.png)

### Uniform Distribution:

We are waiting a phone call. (yay! 😱) Call will come between 2p.m. and 7p.m., all times with the same possibility. What is the possibility, that we will get it before 4p.m.?

> X = what is the current time

$P(X < 4) = ?$

$$P(X < 4) = F(4) =
\begin{cases}
0,  & \text{x ≤ A} \\
{\frac{x-A}{B-A}}, & \text{A < x ≤ B} \\
1,  & \text{B < x} \\
\end{cases} = 
\begin{cases}
0,  & \text{x ≤ 2} \\
{\frac{x-2}{7-2}}, & \text{2 < x ≤ 7} \\
1,  & \text{7 < x} \\
\end{cases} = 
{\frac{4-2}{7-2}} =
{\frac{2}{5}} =
0,4
$$

### Exponential Distribution:

In the Ministry of Silly Walks, there are usually 12 visitors per hour. What is the possibility, that 10 minutes pass without any visitors coming in?

> X = what is the passing time amount

$P(X > 10) = 1 - F(10)$

Usually 12 visitors come in an hour. So time passing between visitors is usually $\frac{60}{12}=5$. This is the $E(X)$, expected value.

$E(X) = \frac{1}{λ} = 5$

$λ = \frac{1}{5} = 0,2$

$$F(10) =
\begin{cases}
0,  & \text{x ≤ 0} \\
{1-e^{-λx}}, & \text{0 < x} \\
\end{cases} = 
{1-e^{-0,2*10}} =
{e^{-2}} =
0,135
$$

### Normal Distribution:

In the Ministry of Silly Walks number of daily clients is describeable by normal distribution. Expected value of daily clients is 560 people, with 40 distribution. What is $P(X<616)$, where $X$ is the number of daily clients.

$E(X) = 560$
$D(X) = 40$

> Of normal distribution, the density function we can not integral, and distribution function it doesn't have.

What to do:

We will make a special Normal Distribution with $E(X)=0$ and $D(X)=1$. It is called **Standard Normal Distribution**. $f(X)$ of it will be:

$ϕ(z) = \frac{1}{\sqrt{2π}}e^{-\frac{z^2}{2}}$

> This density function is also called **Gauss curve**, which full territory is 1

It's $F(X)$ will be values of a table with name of $Φ(z)$:

![Continous Probability Distribution 3](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_3.png)

The **EU** version counts the integral from $-∞$, the **USA** one from 0. Let's not get confused, when we see different values for the same $Φ(z)$. There is always a 0,5 difference (because American counts from 0, which is at half... full $ϕ(z)$ is 1, so half is 0,5).

soooooo.......

$P(X<616) = F(616) = ϕ(\frac{616-μ}{σ}) = ϕ(\frac{616-560}{40}) = ϕ(1,4) = 0,9192$
