# Marginal Distribution and Distribution Formulas

![Common and Marginal Distributions 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/common-and-marginal-distribution_1.png)

So we still have the common, and marginal distributions of balls, we pick from a box.

### Marginal Distribution Formula

> We move let's say from bottom, descending, and always add up the P(X)-es, and get 1 in the end... place under the trendline is possibility for given value

For $X$:

$$   F_X(x) = P(X<x) =
\begin{cases}
{0},  & \text{if $x$ $\leq$ 0} \\
{0,3},  & \text{if 0 $\lt$ $x$ $\leq$ 1} \\
{0,9}, & \text{if 1 $\lt$ $x$ $\leq$ 2} \\
1  & \text{if 2 $\lt$ $x$} \\
\end{cases} $$

For $Y$:

$$   F_Y(y) = P(Y<y) =
\begin{cases}
{0},  & \text{if $y$ $\leq$ 0} \\
{0,6},  & \text{if 0 $\lt$ $y$ $\leq$ 1} \\
1  & \text{if 1 $\lt$ $y$} \\
\end{cases} $$

For $X$ and $Y$:

> their common marginal distribution ^^

$$   F(x,y) = P(X<x,Y<y) =
\begin{cases}
{0},  & \text{if $x$ $\leq$ 0 or $y$ $\leq 0$} \\
{0,1},  & \text{if 0 $\lt$ $x$ $\leq$ 1 and 0 $\lt$ $y$ $\leq 1$} \\
{0,5},  & \text{if 1 $\lt$ $x$ $\leq$ 2 and 0 $\lt$ $y$ $\leq 1$} \\
{0,6},  & \text{if 2 $\lt$ $x$ and 0 $\lt$ $y$ $\leq 1$} \\
{0,3},  & \text{if 0 $\lt$ $x$ $\leq$ 1 and 1 $\lt$ $y$} \\
{0,9},  & \text{if 1 $\lt$ $x$ $\leq$ 2 and 1 $\lt$ $y$} \\
1  & \text{if 2 $\lt$ $x$ and 1 $\lt$ $y$} \\
\end{cases} $$
