# Conditional Possibilities

![Common and Marginal Distributions 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/common-and-marginal-distribution_1.png)

So we still have the common, and marginal distributions of balls, we pick from a box.

Let's calculate some funky values:

$P(X=1,Y=1) = 0,2$

$P(X>0,Y=0) = 0,4+0,1=0,5$

Now let's spice it with [Conmditional Possibilities](https://github.com/ernestdolog/probability-theory/tree/main/2-classical-possibilities/conditional-possibility):

$P(A|B) = {P(A \cap B) \over P(B)}$

$P(X=2|Y=0) = 1 \over{6}$

$P(X<2|Y=0) = 5 \over{6}$

$P(Y=1|X>0) = 2 \over{7}$

$E(X|Y=0) = 0\times{0,1}+1\times{0,4}+2\times{0,1} \over{0,6} = 1$

$E(X|Y=1) = 0\times{0,2}+1\times{0,2}+2\times{0} \over{0,4} = 0,5$

$E(Y|Y=0) = 0\times{0,1}+1\times{0,2} \over{0,3} = 2\over{3}$