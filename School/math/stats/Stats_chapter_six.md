#stats

Area under curve represents probability, from 0 to 100%
# Standard Normal Distribution

## Z-Score Charts
![](POSZ.pdf)
![](NEGZ.pdf)

with calculator, use `normalcdf(-inf, z-score, 0, 1)` to get the area from -inf to a on the normal distribution

Z score formula
$$ z = \frac{x - \mu}{\sigma} $$
where $\mu$ is the mean & $\sigma$ is the standard deviation

for areas in between z scores
$$P(a < z < b) = P(z < b) - P(z < a) $$

with calculator, use `invNorm(area, 0, 1 direction)` to transform an area back into a z-score

==Central Limit Theorem== is typically used for sample sizes over 30, which are not normally distributed, or that are less than 30, but still more than one, and normally distributed.
$$Z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}$$
where $\bar{x}$ is the mean you're looking for and $n$ is the sample size

==Normal Distribution As An Approximation To Binomial==: Is used when sample size $n$ is too large to compute using just the Binomial Distribution

Requirements:
1. You must have a simple random size of $n$
2. $np \ge 5$ and $nq \ge 5$ where $p$ is the probability of success and $q$ is the probability of failure and $q = 1 - p$

Continuity Corrections:
1. $P(X \ge y) \rightarrow P(X > y - 0.50)$
2. $P(X > y) \rightarrow P(X > y + 0.50)$
3. $P(X \le y) \rightarrow P(X < y + 0.50)$
4. $P(X < y) \rightarrow P(X < y - 0.50)$
5. $P(X = y) \rightarrow P(y - 0.50 < X < y + 0.50)$
	* Use this one for ranges in between values as well

Binomial Parameters
1. Mean: $\mu = np$
2. Standard Deviation: $\sigma = \sqrt{n*p*q}$

(for binomial problems, use these definitions of mean and standard distribution)