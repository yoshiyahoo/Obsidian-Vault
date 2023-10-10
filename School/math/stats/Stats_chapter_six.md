#stats

Area under curve represents probability, from 0 to 100%
# Standard Normal Distribution

## Z-Score Charts
![](POSZ.pdf)
![](NEGZ.pdf)

with calculator, use `normalcdf(-inf, z-score, 0, 1)` to get the area from -inf to a on the normal distribution

for areas in between z scores
$$P(a < z < b) = P(z < b) - P(z < a) $$

with calculator, use `invNorm(area, 0, 1 direction)` to transform an area back into a z-score

==Central Limit Theorem== is typically used for sample sizes over 30, which are not normally distributed, or that are less than 30, but still more than one, and normally distributed.
$$Z = \frac{\bar{x} - \mu}{\frac{\sigma}{\sqrt{n}}}$$
where $\bar{x}$ is the mean and n is the sample size