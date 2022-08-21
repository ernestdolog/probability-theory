# Discrete Probability Distributions

> Discrete means, our probability variable is a discrete variable. Something, what can be only described by integers. For example we examine the **number of** faulty products. Or **how many** products a sales agent sold.

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

$P(X=k) = \binom{n}{k} \cdot p^{k} \cdot (1-p)^{n-k}$

where:

n = number of all events

k = number of seeked/expected event

p = possibility of seeked/expected event


**Now let's take an other example:**

In a road, from 30 days usually 12 days there is an accident. What is the possibility, that in a given week, there are 2 days where accident happens?

> Note the word **usually**, so a possibility, a %-ish value is known, and it's **finite**, meaning there can't be more than 7 accident days -> it's **binomial**

$P = \frac{12}{30} = 0,4$

k = 2

n = 7

$P = \binom{7}{2} \cdot 0,4^{2} \cdot (1-0,4)^{7-2}$

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


**Now let's take an other example:**

In a road, from 30 days 12 days happened an accident. What is the possibility, that in a given week, there are 2 days where accident happens?

> It is hypergeometrical, because the de facto N, K, n, k are known

N = 30

K = 12

n = 7

k = 2

$P(X=2) = \frac{\binom{12}{2}\cdot \binom{30-12}{7-2}}{\binom{30}{7}}$


### Poisson Distribution:

In a road, from 30 days **usually 12 accident happens**. What is the possibility, that in a given week, there are 2 days where accident happens?

> Note the word **usually**, so a possibility, a %-ish value is known, and it's **infinite**, because even 100 can happen a day -> it's **poisson**

$P(X=k) = \frac{λ^{k}}{k!} \times e^{-λ}$

X = number of accidents

λ = expectedly how much accidents are in a week

$P(X=2) = \frac{2,8^{2}}{2!} \times e^{-2,8}$

#### Difference Between Binomial and Hypergeometrical:

**Forget about the reverse or random sampling**, as it's not always the case.

Difference is, that in **Binomial Distribution** we know the **possibility** of the seeked/expected event, what is some sort of % value. (take the dice... we throw yellow with possibility of $\frac{2}{6}$) In **Hypergeometrical Distribution** we know the **number of** seeked/expected elements. (we have 2 yellow balls). It seems like the difference here is the reverse/random. But not... let's have 2 examples to clarify:


1) We have a barn where we have 100 fluffy friends, from them 60 are #sheepings. From them we choose 10. What's the possibility, that from the 10, 7 are #sheepings.


2) We have a barn where 60% of fluffy friends are #sheepings. From them we choose 10. What's the possibility, that from the 10, 7 are #sheepings.


Both examples are both random sampling. As we pick 10 fluffy friends. Still, in the first we know the **number of** seeked/expected elements, and second we know the **possibility** of the seeked/expected event. So first is **Hypergeometrical Distribution**, second is **Binomial Distribution**.


#### Difference Between Binomial and Poisson:

Both cases we know some % value. Wording must be expectedly, usually, something like this. 

Difference is: In **Binomial** we have finite events, in **Poisson** infinite. Finite means, that the number of that event happening logically has an upper limit. One week for example can't have more than 7 weeks.


![Discrete Probability Distribution 1](https://github.com/ernestdolog/probability-theory/blob/main/assets/discrete_probability_distribution_1.png)