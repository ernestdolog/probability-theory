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

How to make density function from distribution function? -> we need to derivate it

Given this Distribution function:

![Distribution Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_3.png)

We can dervate all parts to make a Density Function:

![Distribution Function](https://github.com/ernestdolog/probability-theory/blob/main/assets/density_function_4.png)

