# Dispersion

At the **expected value** section we made a case study about an investment idea of putting 30 EUR on roulette. This investment has an $E(X)$ of $29,54 EUR$. We stated that this **excepted value** thingy is a value what possible outcomes will be situated around...

but with what dispersion?

Dispersion: $D(X)$

and:

$D(X) = \sqrt{E(X^2) - E^2(X)}$

Okay, so what does this mean?

Second momentum: $E(X^2)=\sum X_i^2 P(X_i)$

$E^2(X)$ means square of **expected value**

So:

$D(X) = \sqrt{E(X^2) - E^2(X)} = \sqrt{40^2 \times 0,487 + 30^2 \times 0,25 + 20^2 \times 0,128 + 0^2 \times 0,135 - 29,54^2} = 13,52$

## Dispersion of Continouos Probability Variables:

Dispersion is calculateable with the same formula as in discrete case. Just with the values of continouos case:

$$E(X^2)=\int_{-\infty}^{+\infty} x^2 \ f(x) \ dx$$

In case of our example of **Continouos Probability Variables** at **expected value** section value would be:

$$E(X^2)=\int_{-\infty}^{+\infty} x^2 \ f(x) \ dx = \int_{-\infty}^{-1} x^{-2} \ dx + \int_{-1}^{0} -x^4-2x^3 \ dx = \left[{\frac{x^{-1}}{-1}}\right]_{-\infty}^{-1} + \left[-{\frac{x^{5}}{5}-2 \times \frac{x^{4}}{4}}\right]_{-1}^{0} + 0 = {\frac{13}{10}}$$

$E^2(X) = (-{\frac{11}{12}})^2$

$D(X)=\sqrt{{\frac{13}{10}}-(-{\frac{11}{12}})^2}=0,678$