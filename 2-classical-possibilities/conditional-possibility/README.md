# Conditional Possibility

This stuff is about the possibility of A in conditions of possibility of B.

Let's take an example:

Throwing with a 6 sided dice...

A event: odd number

$ P(A) = {3 \over 6} $

> {1, 3, 5}

B event: greater than 3

$ P(B) = {3 \over 6 }$

> {4, 5, 6}

How big is the possibility of A, **in condition** that we know that B surely happens?

It means, we have to reduce all elementary events to `{4, 5, 6}`, because we know B happens.

so $ P(A)_new = {1 \over 3} $

We have a sign for this:

$ P(A|B) = {P(A \cap B) \over P(B)} $

## A situation:

### In a city from 1000 people, exactly 350 consume fast food regularly, and exactly 120 have some circulatory disorder. Exactly 400 people belongs to at least one category. If one person has circulatory disorder, how big possibility we got that he consumes fast food regularly?

$ P(A) = {350 \over 1000} = 0,35$

$ P(B) = {120 \over 1000} = 0,12 $

$ P(A \cup B) = {400 \over 1000} = 0,4$

$ P(A \cup B) = P(A) + P(B) - P(A \cap B)$

$ 0,4 = 0,35 + 0,12 - P(A \cap B)$

$ P(A \cap B) = 0,07$

$ P(A|B) = {P(A \cap B) \over P(B)} $

$\color{green} P(A|B) = {0,07 \over 0,12} = 0,58$