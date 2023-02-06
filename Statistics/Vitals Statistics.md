
## Frequency

Décompte du nombre d'élements dans un groupe particulier ou dans une intervalle

## Cumulative frequency

La somme des fréquences jusqu'à une certaine valeur

## Mean
$$\mu = \frac{\Sigma x}{n}$$
## Mode

Élement dont la valeur est la plus représentée dans le dataset

## Range
$$upperbound - lowerbound$$
## Variance 

$$\frac{\Sigma(x-\mu)^2}{n}$$
ou
$$\frac{\Sigma x^2}{n}-\mu^2$$


## Z-Score

$$z = \frac{x-\mu}{\sigma}$$
## Linear transforms

### Expectations

$$E(aX+b) = aE(X)+b$$

### Variance
$$Var(aX+b) = a^2Var(X)$$

## Permutations
sensible à l'ordre
$$ ^nP_r = \frac{n!}{(n-r)!}$$
## Combinations

$$^nC_r = \frac{n!}{r!(n-r)!}$$

## Geometric Distribution
Prob du premier succès en r essais: $P(X = r) = pq^{r-1}$
Prob d'avoir besoin de plus de r essais pour réussir: $P(X > r) = q^r$
Prob d'avoir besoin de essais ou moins pour réussir: $P(X \leq r) = 1 -q^r$
Esperance: $E(X) = 1/p$
Variance: $Var(X) = q/p^2$

## Binomial Distribution
Use the binomial distribution if you’re running a fixed number of independent trials, each one can have a success or failure, and you’re interested in the number of successes or failures

$$P(X=r) = ^nC_r \times p^r \times q^{n-r}$$
Esperance: $E(X) = np$
Variance: $Var(X) = npq$

## Poisson Distribution
Covers situations where:
- Individual events occur at random and independently in a given
interval. This can be an interval of time or space—for example,
during a week, or per mile.
- You know the mean number of occurrences in the interval or the
rate of occurrences, and it’s finite. The mean number of occurrences
is normally represented by the Greek letter λ (lambda).

$$P(X = r) = \frac{e^{-\lambda} \lambda^r}{r!}$$
Où e = constante d'Euler = 2.718

Esperance: $\lambda$
Variance: $\lambda$
