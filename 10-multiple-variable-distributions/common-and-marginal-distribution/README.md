# Common and Marginal Distributions

Here is a box with 5 balls of multiple colors:

![Common and Marginal Distributions 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/common-and-marginal-distribution_2.png)

We are choosing 2 of them. 

$X = \text{number of picked blue balls}$

$Y = \text{number of picked red balls}$

![Common and Marginal Distributions 2](https://github.com/ernestdolog/probability-theory/blob/main/assets/continous_probability_distribution_1.png)

This is calculated with the help of [combinatorics](https://github.com/ernestdolog/probability-theory/tree/main/1-combinatorics#there-are-20-people-who-can-win-5-sort-of-gifts-how-many-ways-is-it-possible-if-one-person-can-only-win-one-gift-but-gifts-are-all-the-very-same).

**Marginal Distribution** is the side value in the table. Distribution of only one variable, where we don't deal with the other. If we add them up by one variable, it will give 1.

### When are variables independent

If the following is true for them:

$P \index{X}(X=n)*P \index{Y}(Y=k)=P(X=n, Y=k)$

for each and any values.

So let's see if variables from the above example are independent:

X = 1, Y = 0:

$P\index{X}(X=1)*P\index{Y}(Y=k)=P(X=1, Y=0) = 0,6*0,6 = 0,4$

Which isn't true. So they aren't independent.
