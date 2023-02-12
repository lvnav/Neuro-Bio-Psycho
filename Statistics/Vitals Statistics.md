
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

### Sur population:
$$\frac{\Sigma(x-\mu)^2}{n}$$
ou
$$\frac{\Sigma x^2}{n}-\mu^2$$
### Sur échantillon
$$\frac{\Sigma(x-\mu)^2}{n-1}$$

## Expectation

$$E(X) = \Sigma xP(X = x)$$

## Variance (probability distribution)

$$Var(X) = E(X-\mu)^2 = \Sigma(x-\mu)^2P(X=x)$$

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

Can be approximated by Poisson when $p<0.1$ and $n>50$
Can be approximated by Normal when $np > 5$ and $nq > 5$ (ne pas oublier la correction de continuité)

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

Can be approximated by Normal when $\lambda > 15$ (don't forget continuous correction)

## Chi 2 

$$\chi^2_\alpha(\nu) = \Sigma \frac{(O-E)^2}{E}$$
$\nu = (numberOfClasses) - (numberOfRestrictions)$
$\alpha=testSignificance$

## Distribution d'échantillons de proportions(Ps)

Espérance: $E(P_s)=p$
Variance = $Var(P_s)=\frac{pq}{n}$

$$P_s forN(p,\frac{pq}{n})$$
Can ben approximated by Normal when $n>30$ (don't forget continuous correction => $\pm1/2n$)