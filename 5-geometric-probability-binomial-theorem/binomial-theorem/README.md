# Binomial Theorem

Here are these more well known functions:

$(a+b)^2 = a^2 + 2ab + b^2$

$(a+b)^3 = a^3 + 3a^2b + 3ab^2 + b^3$

And less well known:

$(a+b)^4 = a^4 + 4a^3b + 6a^2b^2 + 4ab^3 + b^4$

They follow some sort of order... write them up a lil more precisely:

$(a+b)^2 = 1a^2 + 2a^1b^1 + 1b^2$

$(a+b)^3 = 1a^3 + 3a^2b^1 + 3a^1b^2 + 1b^3$

$(a+b)^4 = 1a^4 + 4a^3b^1 + 6a^2b^2 + 4a^1b^3 + 1b^4$

So those multiplying numbers follow Pascal triangle:

$$\newcommand\cn[2]{\llap{#1}\rlap{#2}\,}
\begin{array}{c}
&&&&&\cn{1}{}&\cn{}{}&\cn{1}{}\\
&&&&\cn{1}{}&\cn{}{}&\cn{2}{}&\cn{}{}&\cn{1}{}\\
&&&\cn{1}{}&\cn{}{}&\cn{3}{}&\cn{}{}&\cn{3}{}&\cn{}{}&\cn{1}{}\\
&&\cn{1}{}&\cn{}{}&\cn{4}{}&\cn{}{}&\cn{6}{}&\cn{}{}&\cn{4}{}&\cn{}{}&\cn{1}{}\\
&\cn{1}{}&\cn{}{}&\cn{5}{}&\cn{}{}&\cn{1}{0}&\cn{}{}&\cn{1}{0}&\cn{}{}&\cn{5}{}&\cn{}{}&\cn{1}{}\\
\end{array}$$

These numbers are called **binomial coefficients**.

So let's see a function how we can calculate binomial coefficients:

$$(a+b)^n=\sum_{k=0}^n {n \choose k} a^{n-k}b^{k}$$

Looks friendly, right?

Let's later figure out some nice python algorythm together to calculate binomial coefficients.