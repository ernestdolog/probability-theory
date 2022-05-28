# Full Possibility Theorem

If we know the conditional possibility of event A for a full event systems all events, the possibility of A is calculateable.

### There are 3 boxes where we have silver and gold coins. All in all 25 silver and 25 gold, all together 50 coins. We mix them into the boxes in a given way shown in the diagram. A fellow is choosing from them. What is his possibility to choose gold?

> Remember, choose from box 1 **OR** from box 2, **OR** from box 3. **OR**: possibilities are added up. :)

![Singly Linked list insert 4](https://github.com/ernestdolog/probability-theory/blob/main/assets/bayes_theorem.png)

So, Full Possibility Theorem says, that: we know all the possibilities of choosing gold coin in the condtion of box 1-3. This way we can count the possibility of choosing a gold coin by itself. This simple. :)

Lets put it now to a lilbit more "maths sounding":

May $B_1, B_2 and B_3$ be a full event system, so they are by pair excluding events, which's Union is the full event system.

> So in our case $B_1, B_2 and B_3$ means if we choose box 1, box 2 or box 3.

So:

$P(A) = P(A|B_1) \times P(B_1) + P(A|B_2) \times P(B_2) + P(A|B_3) \times P(B_3)$

# Bayes Theorem

### There is a grocery shop which gets apples from 3 sources. From the first place he gets 20%, where all apples are good. From the second he gets 30%, from which 5% is bad. From the 3rd place he gets the rest 50%, but here 15% is bad. W choose an apple which is bad, what is the possibility that it is from the 3rd source?

What is the thought here?

Apples come from sources: 20%, 30%, 50%

But as we know that the event that the apple is bad is certain, so possibilities change:

0%, 25%, 75%

This is where Bayes Theorem comes to help us: We would like to calculate the possibility of an earlier happened $B_k$ event in the condition of a later happened A event.

May $B_1, B_2 ... B_n$ be a full event system, and A as a random event. So for any $B_k$ event:

$$ P(B_k|A) = {{ P(A|B_k) \times P(B_k) } \over {\sum_{n=1}^n P(A|B_n) \times P(B_n)}} = {{ P(A|B_k) \times P(B_k) } \over {P(A|B_1) \times P(B_1) + P(A|B_2) \times P(B_2) + P(A|B_3) \times P(B_3) + ... + P(A|B_n) \times P(B_n)}} $$

