#stats 

==Probability Distribution==: A table which contains a random variable "X", which represents numbers along with their corresponding probabilities "P(X)". The sum of all these probabilities must be 1.

### Formulas for probability distributions
1. Mean: $\mu = \sum_{}^{}{X * P(X)}$
2. Variance: $\sigma^2 = \sum_{}^{}{(X - \mu)^2 * P(X)}$
3. Standard Deviation: $\sigma = \sqrt{\sum_{}^{}{(X - \mu)^2 * P(X)}}$


==Binomial Process==: a process in which only "2" outcomes are possible; either a success or a failure
Examples: 
1. Answering true or false on a test
2. Turning on or off a light
3. Scoring a touchdown or not scoring one

==Binomial Experiment==
1. Each trial is fixed
2. Each trail is independent, meaning that the outcome of one does not affect the outcome of the others
3. Each outcome is either a success or a failure
4. The probability of success must remain the same throughout the experiment

==Expected Value==:
value that is "expected" in games such as gambling or insurance. NET amount of money earned
$\mu = E(X) = \sum_{}^{}{X * P(X)}$

==Binomial Formula==:
$$p(x) = \frac{n!}{(n-x)! * x!} * p^x * q^{n - x}$$
where n is the number of trials, x are the number of successes, p is the probability of success, and q is the probability of failure where $q = 1 - p$

use `binompdf(# trails, probability, # successes)` (binomial probability) in calculator to calculate exact values 

use `binomcdf(# trails, probability, #successes)` (binomial cumulative probability) in calculator to calculate less than or equal to x successes in n trials

### Formulas for binomial experiment
1. Mean: $\mu = n * p$
2. Variance: $\sigma^2 = n * p * q$
3. Standard Deviation: $\sigma = \sqrt{n * p * q}$
