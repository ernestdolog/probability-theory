# Expected Value

An example:

We take 3 pieces of 10 EUR bank notes, and we plan to invest them. With the help of a Roulette table.

> 1 green, 18 red, 18 black fields,

Our business model looks like this:
- If we win, we win +10 EUR to the existing 10 EUR.
- We put 10 EUR on the red, if win that's it, we finish
- If not win, we put other 10 EUR on red, and so on until the 3rd bank note.

In case of the first win we always get out the game.

What is the expected return of our investment?

This is the formula of **expected value**:

$E(X)=\sum X_i \times P(X_i)$

Let's draw a little:

![Expected Value](https://github.com/ernestdolog/probability-theory/blob/main/assets/expected_value_1.png)

So, let's use our formula:

$E(X)=\sum X_i \times P(X_i) = 40 \times 0,487 + 30 \times 0,25 + 20 \times 0,128 + 0 \times 0,135 = 29,54$

It does not mean that we can count with exactly this value. It means that exact values what can come out will be around this number.

So, this might not be a startup idea.