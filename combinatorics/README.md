# Combinatorics

This thingy is about how many ways do we differentiate in equally possible choices of n choosable in x combinations.

> For example how many ways can we seat 5 people in 5 places:

```
x <- 5
x <- 4
x <- 3
x <- 2
x <- 1
------------
5*4*3*2*1
```

### General tip when tackling combinatorics:
We multiply and we add sometimes. When to multiply, when to add?:
```
apple
apple
apple

lemon
lemon
------------
- choose 1 apple **AND** 1 lemon
3*2
- choose 1 apple **OR** 1 lemon
3+2
```
Try to express what we want in words, using **AND**/**OR**. **AND** indicates multiplication, **OR** indicates addition. This simple.

## Main topics:

### Permutation:
> How many ways can 5 people sit down in 5 seats?

\$$ 5\times4\times3\times2\times1 = 5!$$

### Variation:
> How many ways can 3 people out of 5 sit down next to each other in a bench?\n
\$$ 5\times4\times3 = 60$$
It is exactly like **Permutation** but here we don't put everyone in, just those who we chose.

\$$ n\times(n-1)\times(n-2)\times...\times(n-k+1) = \sum_{k=1}^n (n-k+1) = {n!  \over(n-k)}$$

> Most pocket calculators have a button for it. `npr` - 5`npr`3 meaning: how many ways can we put 3 out of 5 ppl next to each other

### Combination:
>

