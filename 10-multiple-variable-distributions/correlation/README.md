# Correlation

![Common and Marginal Distributions 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/common-and-marginal-distribution_1.png)

So we still have the common, and marginal distributions of balls, we pick from a box.

Let's calculate some funky values:

$E(X) = 0 \times{0,3} + 1 \times{0,6} + 2 \times{0,1} = 0,8$

$E(Y) = 0 \times{0,6} + 1 \times{0,4} = 0,4$

$E(X /times{Y}) = \sum{X\times{Y}\times{P(X\times{Y})}} = 0 \times{0} \times{0,1} + 1 \times{0} \times{0,4} + 2 \times{0} \times{0,1} + 0 \times{1} \times{0,2} + 1 \times{1} \times{0,2} + 2 \times{1} \times{0} = 0,2$

and now some distributions, just to feel the vibe! 🦄

$D(X) = \sqrt{E(X^{2})-E^{2}(X))} = ...$

wut?

$E(X^{2}) = \text{second momentum} = 0^{2} \times{0,3} + 1^{2} \times{0,6} + 2^{2} \times{0,1} = 1$

$E^{2}(X) = E(X)^{2} = 0,8^{2} = 0,64$

so:

$D(X) = \sqrt{1 - 0,64} = 0,6$

$D(Y) = \sqrt{0,4 - 0,16} = 0,4899$

$COV(X,Y) = E(X \times{Y}) - E(X)\times{E(Y)} = 0,2 - 0,8 \times{0,4} = -0,12$

$R(X,Y) = E(X \times{Y}) - E(X)\times{E(Y)} = 0,2 - 0,8 \times{0,4} = -0,12$

$R(X,Y) = {COV(X,Y) \over D(X)\times{D(Y)}} = {-0,12 \over 0,6\times{0,4899}} = -0,4083$

 - Correlation describes the relation between X and Y. It's a number ideally between -1 and 1. 

 - If correlation is between -0,5 and 0,5, relation is weak.

 - If correlation is negative, relation is reverse/