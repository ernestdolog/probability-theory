# Combinatorics

This thingy is about how many ways stuff can happen? How many possible variations we got?

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

$$ 5\times4\times3\times2\times1 = 5!$$
### Variation:
> How many ways can 3 people out of 5 sit down next to each other in a bench?

$$ 5\times4\times3 = 60$$

It is exactly like **Permutation** but here we don't put everyone in, just those who we chose.

$$ n\times(n-1)\times(n-2)\times...\times(n-k+1) = \sum_{k=1}^n (n-k+1) = {n!  \over(n-k)}$$

> Most pocket calculators have a button for it. `npr` - 5`npr`3 meaning: how many ways can we put 3 out of 5 ppl next to each other

### Combination:
> How many ways can we choose 3 people out of 5.

$$ {5 \choose 3}$$

Funfact:

$$ {5 \choose 3} = {5 \choose 2}$$

Because if you would like to choose 3 fingers in one of your hand, you already choose 2.

> Most pocket calculators have a button for it. `ncr` - 5`ncr`3 meaning: how many ways can we choose 3 out of 5 ppl

$$ {n \choose k} = {n! \over k!(n-k)!}$$

## Some situations it comes handy:

### There are 20 people travelling in a bus at a point of time. The bus at this point of time have 5 stops to come. Through this following 5 stops all passengers leave the bus. How many variations can it happen?

- here are the stops:

```
x <- 20 people can possibly leave
x <- 20 people could possibly leave, but we have NO CLUE how many left at the previous step
x 
x 
x 
```

Seemingly at the second step we got a problem. Here comes a **handy tip**:
> Whenever we are trying to solve smth with combinatorics, and we can't provide a solution. Solve it with **a chainsaw**. Either by turning around the problem. (turning around what do i order to what, f ex i used to render the passengers to the stops -> so than let's render the stops to the passengers ^^)

```
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
x <- 5 stops he can choose from
...
x <- 5 stops he can choose from
```

So what did we agree upon **multiplication** and **addition**?: Passenger 1 can choose between 5 stops **AND** passenger 2 can ...

so:

$$ 5\times5\times5\times5\times...\times5 = 5^20$$