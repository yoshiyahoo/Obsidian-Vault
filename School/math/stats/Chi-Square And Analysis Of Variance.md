# Goodness Of Fit Test
Apply hypothesis test to observe the frequencies ("O") of some values listed in a one-way frequency table.
* Interested to see how vars fit in a claimed distribution

* Assume Right Tailed Test
* Use Chi Square

Test Statistic:
$\chi^2 = \sum_{}\frac{(O-E)^2}{E}$
where $O$ is the "Observed" frequencies from the chart and $E$ is the mean of the expected frequencies
* $df$ is the number of observed frequencies - 1

# Contingency Table
Two - way frequency table consisting of counts of categorical data. Corresponds to two different variables

Apply Hypothesis Test
- Assumed RIGHT-TAILED
- Use Chi square
- $df$ are (# of rows - 1) * (# of columns - 1)
- Independent variables involve $=$, dependent (related) involves a NOT equal $\ne$ 

Test Statistic:
$\chi^2 = \sum_{}\frac{(O-E)^2}{E}$
* where $E = \frac{\text{Row Sum} * \text{Column Sum}}{\text{Sum of all observed frequencies}}$ is the *expected value*
* $\frac{(O-E)^2}{E}$ is the square Pearson Residual
* Each Cell In the Table has it's own E & O value

# Analysis Of Variance (ANOVA)
* equality or difference between *THREE or more population means*
* describes one feature from three or more different samples

## Testing With Hypothesis Test
1. Claim $\mu_1 = \mu_2 = \mu_3$ for equality or $\mu_1 \ne \mu_2 \ne \mu_3$ for difference
2. $H_0: \mu_1 = \mu_2 = \mu_3$, $H_1: \mu_1 \ne \mu_2 \ne \mu_3$ (Assume RIGHT TAILED TEST)
3. apply F - distribution
4. Find test statistic
$$F = \frac{n * s_\bar{x}^2}{s_p^2}$$
* n is the sample size of each of the three or more groups
* $s_\bar{x}^2 = \sum_{}\frac{(x_i - \bar{x})^2}{n - 1}$ is the variance of the sample means of each group
* $s_p^2 = \sum_{}s_i^2$ where $s_i^2 = \sum_{}\frac{(x_i - \bar{x}_i)^2}{n - 1}$ is the mean of each sample variance from the groups
* On calculator, enter data as lists. Then go to `stat` `tests`, `ANOVA`, then put in your three lists. Then press enter

5. Find critical values using F-distribution table, There will be degrees of freedom of the numerator $d_{fn} = k - 1$ where k is the # of groups being tested. Degrees of freedom in denominator $d_{fd} = k * (n - 1)$
6. Find P value using technology, use the `Fcdf(test stat, 9999999, dfn, dfd`
7. Check if P value is less than or equal significance level $\alpha$, if so, reject $H_0$, otherwise, fail to reject $H_0$
