# Distribution Function

Let's say a fellow shoots to a target. Radius of the target is 50cm, he shoots `X`cm from the target. X is called variability.

He surely hits the target. Let's calculate the possibility that he hits the inner 10cm radius area.

$\color{orange} P(X<10) = ?$

$T = r^2 \times π$

$P(X<10) = {10^2 \times π} \over {50^2 \times π} = {1 \over 25}$

$P(X<20) = {20^2 \times π} \over {50^2 \times π} = {4 \over 25}$

$P(X < x) = {x^2 \times π} \over {50^2 \times π}$

This is meaning that the possibility of the fellow hits into a given radius circle in a 50cm redius target is such...

But, it has edge values:
 - x can't be smaller than 0
 - if it is bigger than the radius of the target -> known the fact he surely hits the target, possibility is 1

let's correct our function:

$   P(X < x) =
\begin{cases}
0,  & \text{if $x$ $\leq$ 0} \\
{x^2} \over {50^2}, & \text{if 0 $\lt$ $x$ $\leq$ 50} \\
1,  & \text{if 50 $\lt$ $x$} \\
\end{cases} $

so what we are getting here is a function, what we can write like this:

$ x \mapsto  P(X < x)$

This function we call the distribution function of $X$ probability variable and sign it with $F(X)$.

> X can be whatever, 12,5... 25,25 and any values... so it is called: continuous probability variable

