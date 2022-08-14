# Binomial and Hypergeometrical Distributions

### Binomial Distribution:

We have a dice where 3 sides are green, 2 sides are yellow, 1 side is red. What is the possibility that we throw 2 yellows after each other?

$P(yellow) = \frac{2}{6}$

So we throw red **and** red. From the forbidden wisdom of [Combinatorics](https://github.com/ernestdolog/probability-theory/tree/main/1-combinatorics#general-tip-when-tackling-combinatorics), we know that **and** means $*$. So possibility of throwing 2 yellow:

$P = \frac{2}{6} \cdot \frac{2}{6}$

Than we also throw 2 non yellow:

$P = \frac{2}{6} \cdot \frac{2}{6} \cdot \frac{4}{6} \cdot \frac{4}{6}$

But this is the possibility of throwing exactly 2 yellow, and than 2 non yellow. We would like to know the possibility of throwing 2 yellows at any place.
So we want to know how many times we can place 2 yellows in 4 throws, that will be:


$P = \binom{4}{2}\cdot \frac{2}{6} \cdot \frac{2}{6} \cdot \frac{4}{6} \cdot \frac{4}{6} = 0,2963$

So this technique we will use so many times, that we give it a name. Because unfortunately it wasn't me, who named it, it didn't become My Little Pony Distribution, or such, but **Binomial Distribution**. And its equity is:

$P = \binom{n}{k} \cdot p^{k} \cdot (1-p)^{n-k}$

where:

n = number of all events
k = number of seeked/expected event
p = possibility of seeked/expected event

### Hypergeometrical Distribution:

In a box we have 3 blue, 2 yellow and 1 red balls. We pick 4 from it. What's the possibility that exactly 1 is yellow?

$P = \frac{expected}{all} = \frac{\binom{2}{1}\cdot \binom{3}{4}}{\binom{6}{4}}$

all: we need to pick 4 balls from 6, how many ways can we do it
expected: we pick 1 from the 2 yellows, and 3 from the 4 non-yellows

We will use this a lot too, so we give a **hyper**good name to it: **Hypergeometrical Distribution**.

general equity:

$P(X=k) = \frac{\binom{K}{k}\cdot \binom{N-K}{n-k}}{\binom{N}{n}}$

N = all elements
K = not seeked/expected elements
n = picked elements
k = picked not seeked/expected elements