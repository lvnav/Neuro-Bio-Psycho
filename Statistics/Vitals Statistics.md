
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

## Bayes

$$P(A|B)=\frac{P(A \cap B)}{P(B)}$$
$$P(A \cap B) = P(A|B) \times P(B)$$
$$P(B \cap A) = P(B|A) \times P(A)$$

Si A et B sont indépendants : $P(A|B) = P(A)$

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

## Distribution d'échantillons de proportions(Ps)

Espérance: $E(P_s)=p$
Variance = $Var(P_s)=\frac{pq}{n}$

$$P_s forN(p,\frac{pq}{n})$$
Can be approximated by Normal when $n>30$ (don't forget continuous correction => $\pm1/2n$)

## Sampling

$\mu$ = mean of population
$\bar{\mu}$ = mean of the sample
$\hat{\mu}$ = point estimator = estimation de la valeur de la pop. à partir d'un échantillon

$\hat{\sigma}^2 =s^2$

We can estimation the population mean by the sample mean => $\bar{\mu} = \hat{\mu}$


## Sampling distribution of means

Espérance = $E(\bar{X})=\mu$
Variance = $Var(\bar{X})=\frac{\sigma^2}{n}$
Écart-type = $\sqrt{Var(\bar{X})}$
Erreur type(Standard error of the mean) = $\frac{\sigma}{\sqrt{n}}$

By the central limit theorem, if your sample of X is
large, then X’s distribution is approximately normal.


$$\bar{X}\sim N(\mu, \frac{\sigma^2}{n})$$
## Confidence interval

$$statistic \pm(marginOfError)$$
where $marginOfError=c\times(standardDeviationOfStatistic)$

1. choose pop statistic to estimate(ex: mean)
2. find its sampling distribution
3. decide level of confidence
4. find confidence limits

| Population Statistic | Population distribution | Conditions| Confidence interval|
|- | - |-|-|
|$\mu$|Normal|Know what $\sigma^2$ is. n is large or small. $\bar{X}$ is the sample mean | $\bar{x}-c\frac{\sigma}{\sqrt{n}},\bar{x}+c\frac{\sigma}{\sqrt{n}}$
|$\mu$|Non-normal|Know what $\sigma^2$ is. n is large (at least 30). $\bar{X}$ is the sample mean  |$\bar{x}-c\frac{\sigma}{\sqrt{n}},\bar{x}+c\frac{\sigma}{\sqrt{n}}$
|$\mu$|Normal or non-normal|Don't know what $\sigma^2$ is. n is large (at least 30). $\bar{X}$ is the sample mean. $s^2$ is the sample variance|$\bar{x}-c\frac{s}{\sqrt{n}},\bar{x}+c\frac{s}{\sqrt{n}}$
|p|Binomial|n is large. $p_s$ is the sample proportion. $q_s$ is $1-p_s$ |$p_s-c\sqrt{\frac{p_sq_s}{n}},p_s+c\sqrt{\frac{p_sq_s}{n}}$

|Level of confidence|Value of c|
|-|-|
|90%|1.64|
|95%|1.96|
|99%|2.58|


## T-Distribution

$T\sim t(v)$

| Population Statistic | Population distribution | Conditions| Confidence interval|
|- | - |-|-|
|$\mu$|Normal or non-normal|Dont know what $\sigma^2$ is. n is small (less than 30). $\bar{X}$ is the sample mean. $s^2$ is the sample variance| $\bar{x}-t(v)\frac{s}{\sqrt{n}},\bar{x}+t(v)\frac{s}{\sqrt{n}}$

## Hypothesis testing
!!!!!!!!!!!S'ENTRAINER !!!!!!!!!

## Chi 2 
$$\chi^2_\alpha(\nu) = \Sigma \frac{(O-E)^2}{E}$$
$O$ = observed frequencies
E = expected frenquencies

$\nu = (numberOfClasses) - (numberOfRestrictions)$
$\alpha=testSignificance$

In a test for independence for two variables, if your contingency table has h rows and k columns:
$ν = (h – 1) × (k – 1)$

| Distribution | Conditions | $\nu$ |
|- | - |-|
|Binomial|You know what p is.<br/><br/> You don't know what p is, and you have to estimate it from the observed frequencies|$v=n-1$<br/><br/>$v=n-2$|
|Poisson|You know what $\lambda$ is.<br/><br/> You don't know what $\lambda$ is, and you have to estimate it from the observed frequencies|$v=n-1$<br/><br/>$v=n-2$|
|Normal|You know what $\mu$ and $\sigma^2$ is.<br/><br/> You don't know what $\mu$ is and $\sigma^2$ are, and you have to estimate it from the observed frequencies|$v=n-1$<br/><br/>$v=n-3$|


$\chi^2$ can be used to testing goodness of fit and independence (with table of contingency)

## Correlation and regression

To make a regression we need to find the equation of the line = $y=a+bx$
SSE = sum of squared errors = $\Sigma(y-\hat{y})^2$

$$b=\frac{\Sigma((x-\bar{x})(y-\bar{y}))}{\Sigma(x-\bar{x})^2}$$
and 
$$a = \bar{y}-b\bar{x}$$
where $\bar{x}$ = mean of $x$ (ditto for $y$)


Correlation
$$r=\frac{bs_x}{s_y}$$