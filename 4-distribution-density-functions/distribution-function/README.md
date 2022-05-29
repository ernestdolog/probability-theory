# Distribution Function

### Let's say a fellow shoots to a target. Radius of the target is 50cm, he shoots `X`cm from the target. X is called variability. He surely hits the target. Let's calculate the possibility that he hits the inner 10cm radius area.

$\color{orange} P(X<10) = ?$

$T = r^2 \times π$

$P(X<10) = {{10^2 \times π} \over {50^2 \times π}} = {1 \over 25}$

$P(X<20) = {{20^2 \times π} \over {50^2 \times π}} = {4 \over 25}$

$P(X < x) = {{x^2 \times π} \over {50^2 \times π}}$

This is meaning that the possibility of the fellow hits into a given radius circle in a 50cm redius target is such...

But, it has edge values:
 - x can't be smaller than 0
 - if it is bigger than the radius of the target -> known the fact he surely hits the target, possibility is 1

let's correct our function:

$$   P(X < x) =
\begin{cases}
0,  & \text{if $x$ $\leq$ 0} \\
{x^2} \over {50^2}, & \text{if 0 $\lt$ $x$ $\leq$ 50} \\
1,  & \text{if 50 $\lt$ $x$} \\
\end{cases} $$

so what we are getting here is a function, what we can write like this:

$ x \mapsto  P(X < x)$

This function we call the distribution function of $X$ probability variable and sign it with $F(X)$.

> X can be whatever, 12,5... 25,25 and any values... so it is called: continuous probability variable

Let's see an other situation:

### 2 people shooting a target. Person 1 has possibility of 0,7 hitting the target, person 2 have 0,8 possibility hitting the target. They shoot 1-1 time. Let's give the distribution function of this situation.

> X can be 0, 1, 2, not whatever... so we call it: discrete probability variable

probabilities of hits:

$ P(0) =  0,3 \times 0,2 = 0,06 $

$ P(1) =  0,7 \times 0,2 + 0,3 \times 0,8 = 0,38 $

$ P(2) =  0,7 \times 0,8 = 0,56 $

These are probabilities... now let's say what will the **distribution function** order to value 3?

Maybe 0? We can't hit 3... **NOPE!**

**Distribution function** orders to each $x$ the $P(X < x)$. (So the cumulative value of everything smaller in this case)

So:

$F(3) = 1$

$F(0) = 0$

$F(1) = 0,06$

$F(2) = 0,44$

**Discrete probability variable** we call all probability variable which can take up countably much possibilities. (it can be taken by concrete given values)