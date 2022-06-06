# Density Function

$f(x)$

> In density function possibilities are given by the area under the Distribution Function.

![Density Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_1.png)

Depending on where we are looking for possibilities, we need to integrate given function in a 1 dimension scale.

> If we want to get how much possibility the event $x=0$ has. It is 0. Let's memorize: if a continouos probability variable takes a concrete value it has 0 possibility.

> But! Where do we know that $x$ is a continouos probability variable? -> **Density Function can only belong to continouos probability variable**

In the drawing we see 3 areas under the function. If we add up their areas it's always 100%, or 1.

$$\int_{-\infty}^{+\infty} f(x) \,dx= 1$$

So...

![Density Function Vlidity Check](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_2.png)

So this function is a valid density function.

There is also smth: it can't be negative... so the graph has to be always over the X dimension, which is also fine in our case.

## Distribution Function -> Density Function

> we need to derivate it as simple than it is

Given this Distribution function:

![Distribution Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_3.png)

We can derivate all parts to make a Density Function:

![Distribution Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_4.png)


## Density Function -> Distribution Function

> We will need to integrate it, but this isn't all...

Let's see the Distribution Function from the last example. Let's integrate it to get back the **exact same** Density Function as e had:

![Problematic Density Function Generation](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_5.png)

It is already 90% nice. But we are **missing the constants**. We need that ${\frac{1}2}$ for example.

Here comes a trick!!! A nice out the box trick...

$$\color{green}F(x)=\int_{-\infty}^{x} f(t) \,dt$$

So, let's understand hat does it mean.

 - $F(x)$ means Distribution Function of variable $x$
 - $\int_{-\infty}^{x}$ means integral of **something**!! from negaitve endless to $x$ (we are looking for Distribution Function of that exact $x$!!!)
 - $f(t) \,dt$ is WTF... what is this $t$ doing, why is it? Why am I?!

> So now we are talking about continouos probability variables. They don't take smth concrete... t is technically the same as $x$. Even practically. We just created this $t$ to emphasize, that we take limits of $x$, and integrate $f(x)$ in those limits, but as a continouos probability variable. So as $x$ kind of lost its continuity, we put this t in place of it, to save it... main thing is the function, not the variable.

So what it will mean in practice for us:

$$   f(x) =
\begin{cases}
e^{2x},  & \text{if $x$ $\leq$ 0} \\
{1-x}, & \text{if 0 $\lt$ $x$ $\leq$ 1} \\
0,  & \text{if 1 $\lt$ $x$} \\
\end{cases} $$

Let's make a correct **Density Function** out of it:

**Case 1:**

> $x$ $\leq$ 0

$$F(x)=\int_{-\infty}^{x} f(t) \,dt = \int_{-\infty}^{x} e^{2t} \, dt = \left[e^{2t}\times {\frac{1}2}\right]_{-\infty}^{x} = e^{2x} \times {\frac{1}2} - e^{-\infty} \times {\frac{1}2} = e^{2x} \times {\frac{1}2} - 0 \times {\frac{1}2} = e^{2x} \times {\frac{1}2}$$

**Case 2:**

> 0 $\lt$ $x$ $\leq$ 1

$$F(x)=\int_{-\infty}^{x} f(t) \,dt = \int_{-\infty}^{0} e^{2t} \, dt + \int_{0}^{x}(1-t) \, dt = e^{2\times0} \times {\frac{1}2} + \left[t - {\frac{t^2}2}\right]_{0}^{x} = {\frac{1}2} + x - {\frac{x^2}2} - 0 = {\frac{1}2} + x - {\frac{x^2}2}$$

For the sake of shortness, I didn't integrate again $\int_{-\infty}^{0} e^{2t} \, dt$, just popped 0 into x from the previous cases Newton Leibniz formula. Keep in mind that intergal in $-\infty$ is a borderline, and it is 0. So in Newton Leibniz formula I don't write $- 0$.

**Case 3:**

> 1 $\lt$ $x$

$$F(x)=\int_{-\infty}^{x} f(t) \,dt = \int_{-\infty}^{1} f(t) \, dt + \int_{1}^{x}0 \, dt = {\frac{1}2} + 1 - {\frac{1^2}2} + 0 = 1$$