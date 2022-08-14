# Big Numbers Theorem

### What is it all about:

To understand this, let's see a little story with **relative commonness**.

We are rolling a dice. $X$ will be the amount of 6 rolls, $n$ will be the amount of all of our rolls.

Relative commonness is $\frac{X }{n}$

So if we roll 1 time, and our roll is a 6, our relative commonness is $\frac{X }{n} = \frac{1 }{1} = 1$ .

If we roll 2 times, and our roll is 6 1 time, and not 6 1 time, our relative commonness is $\frac{X }{n} = \frac{1 }{2} = 0.5$ .

Let's collect possible relative commonnesses of our experiment for a couple of $n$-s.:

![Big Numbers Theorem 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/big_numbers_theorem_1.png)

The more we are rolling the dice, we have more and more chance, that relative commonness ( $p$ ) will be a number around $\frac{1 }{6}$ . Because $\frac{1 }{6}$ is
the theoretical probability of the event that we roll a 6.

Big Numbers Theorem is about this.

### What it is in fact:

If an event's outcome possibility is $p$, the more we are doing the experiment, relative commonness and theoritical possibility will have smaller and smaller difference.

$P\left ( \left | \frac{X}{n} - p \right | < \varepsilon  \right ) \geq 1 - \frac{p  (1-p) }{n\varepsilon ^2}$


$P\left ( \left | \frac{X}{n} - p \right | >  \varepsilon  \right ) < 1 - \frac{p  (1-p) }{n\varepsilon ^2}$

Character $\varepsilon$ means the "mistake" - difference between relative commonness and theoretical probability.

### An example:

How many times do we need to roll a dice, so the possibility of rolling 6 would be in 0.1 precision range of relative commonness in 95% of cases?

so let's see what we got:

- $n$ -> how many we need to roll
- $p = \frac{1}{6}$, the relative commonness
- $\varepsilon\varepsilon = $ 
- 95% we call as **confidence level**: $1 - \frac{p  (1-p) }{n\varepsilon ^2}$ - right side of our equity

And than, let's use our wonderful tools:


$P\left ( \left | \frac{X}{n} - p \right | < \varepsilon  \right ) \geq 1 - \frac{p  (1-p) }{n\varepsilon ^2}$

$P\left ( \left | \frac{X}{n} - \frac{1}{6} \right | < 0,1 \right ) \geq 1 - \frac{\frac{1}{6}  (1-\frac{1}{6}) }{n*0,1^{2}}$

using **confidence level**

$1 - \frac{\frac{1}{6}  (1-\frac{1}{6}) }{n*0,1^{2}} = 0,95$

n = 277,78

