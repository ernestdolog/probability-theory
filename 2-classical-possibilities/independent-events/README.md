# Independent events

All events we call independet where this applies: $ P(A \cap B) = P(A) \times P(B) $


Let's take an example:

Throwing with a 6 sided dice...

A event: greater than 2

$ P(A) = {4 \over 6} $

> {3, 4, 5, 6}

B event: odd number

$ P(B) = {3 \over 6 }$

> {1, 3, 5}

$\color{green}P(A \cap B) = {2\over 6} = {3\over 6} \times {4\over 6}$

> {4, 6}

> The above means: A and B are independent, if their common possibility is the only and only combined event when **A AND B happens** (AND: multiplication, remember! :) )

Now let's see smth else:

C even: we throw 3 or 5

Are B and C independent?

$ P(B \cap C) = P(B) \times P(C) $

$\color{red} {2\over 6} = {3\over 6} \times {2\over 6} $

So B and C events aren't indeendent events. :)

> The above means: Throwing an odd number, or throwing 3 or 5 are not independent events. Later event is part of the previous event. Always try to model problems down to simple, down to earth words. :))


## A situation:

### An insurance company have many clients. 70% has car insurance, 60% has home insurance, 90% has at least 1 from car or home insurance. Are these events independent from each other?

$ P(A) = 0,7 $

$ P(B) = 0,6 $

$ P(A \cup B) = 0,9 $

$ P(A \cup B) = P(A) + P(B) - P(A \cap B) $

$ 0,9 = 0,7 + 0,6 - P(A \cap B) $

$ P(A \cap B) = 0,4 $

$\color{red} 0,42 = 0,7 \times 0,6 \neq 0,4 $

So these event are **NOT INDEPENDENT**.

### An insurance company have many clients. 70% has car insurance, 20% has home insurance and no car insurance, how many percent has car insurance, if we know that car insurance and home insurance are independent events?

$ P(A) = 0,7 $

$ P(B) = ? $

$ P(B\A) = P(B) - P(B \cap A) = 0,2 $

$ 0,2 = P(B) - 0,7 \times P(B)$

$ {0,2 \over P(B)} = 1 - 0,7 = 0,3$

$ 0,2 = 0,3 \times P(B)$

$\color{green}  {2 \over 3} = P(B)$