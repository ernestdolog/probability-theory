# Expected Value

An example:

We take 3 pieces of 10 EUR bank notes, and we plan to invest them. With the help of a Roulette table.

> 1 green, 18 red, 18 black fields,

Our business model looks like this:
- If we win, we win +10 EUR to the existing 10 EUR.
- We put 10 EUR on the red, if win that's it, we finish
- If not win, we put other 10 EUR on red, and so on until the 3rd bank note.

In case of the first win we always get out the game.

What is the expected return of our investment?

This is the formula of **expected value**:

$E(X)=\sum X_i \times P(X_i)$

Let's draw a little:

![Expected Value](https://github.com/ernestdolog/probability-theory/blob/main/assets/expected_value_1.png)

So, let's use our formula:

$E(X)=\sum X_i \times P(X_i) = 40 \times 0,487 + 30 \times 0,25 + 20 \times 0,128 + 0 \times 0,135 = 29,54$

It does not mean that we can count with exactly this value. It means that exact values what can come out will be around this number.

So, this might not be a startup idea.

## Expected Value of Continouos Probability Variables:

This case:

$$E(X)=\int_{-\infty}^{+\infty} x \times f(x)\ dx$$

Let's see an example... here is a $f(x)$ density function:

$$   f(x) =
\begin{cases}
{\frac{1}{x^4}},  & \text{if $x$ $\leq$ -1} \\
{-x^2-2x}, & \text{if -1 $\lt$ $x$ $\leq$ 0} \\
0,  & \text{if 0 $\lt$ $x$} \\
\end{cases} $$

Let's calculate it's **expected value**:

![Expected Value Density Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/expected_value_2.png)

So as our formula says:

$$E(X)=\int_{-\infty}^{+\infty} x \times f(x)\ dx= \int_{-\infty}^{-1}x \times {\frac{1}{x^4}}\ dx + \int_{-1}^{0}x \times({-x^2-2x})\ dx +  \int_{0}^{+\infty}x \times 0\ dx = \left[{\frac{x^{-2}}{-2}}\right]_{-\infty}^{-1} + \left[-{\frac{x^{4}}{4}-2 \times \frac{x^{3}}{3}}\right]_{-1}^{0} + 0 = -\frac{1}{2}+ \ -\frac{5}{12} = -\frac{11}{12}$$
