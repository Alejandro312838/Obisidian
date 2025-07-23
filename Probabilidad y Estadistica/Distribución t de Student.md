The _t_-distribution is a type of normal distribution that is used for smaller sample sizes. Normally-distributed data form a bell shape when plotted on a graph, with more observations near the mean and fewer observations in the tails.

The _t_-distribution is used when data are _approximately_ normally distributed, which means the data follow a bell shape but the population variance is unknown
Grafico de la distribucion:
![[{886FDA77-24F8-4FCD-AE7C-8588BC3E97C6}.png]]
As the degrees of freedom (total number of observations minus 1) increases,
the t-distribution will get closer and closer to matching the standard normal
distribution, a.k.a. the z-distribution, until they are almost identical.

`Above 30 degrees of freedom, the _t_-distribution roughly matches the _z_-distribution. Therefore, the _z_-distribution can be used in place of the _t_-distribution with large sample sizes.`

`The _z_-distribution is preferable over the _t_-distribution when it comes to making statistical estimates because it has a known variance. It can make more precise estimates than the _t_-distribution, whose variance is approximated using the degrees of freedom of the data.`

#### Distribucion T y valores t
A t-score is the number of standard deviations from the mean in a t-distribution.
You can typically look up a t-score in a t-table, or by using an online t-score
calculator.

Usos de los valores t
1. The upper and lower bounds of a confidence interval when the data are approximately normally distributed.
2. The _p_-value of the test statistic for _t_-tests and regression tests.

### _T_-scores and confidence intervals

Confidence intervals use _t_-scores to calculate the upper and lower bounds of the prediction interval. The _t_-score used to generate the upper and lower bounds is also known as the **critical value** of _t_, or _t_*.

### _T_-scores and _p_-values

Statistical tests generate a [test statistic](https://www.scribbr.com/statistics/test-statistic/) showing how far from the null hypothesis of the statistical test your data is. They then calculate a [_p_-value](https://www.scribbr.com/statistics/p-value/) that describes the likelihood of your data occurring if the null hypothesis were true.

The _t_-score which generates a _p_-value below your threshold for [statistical significance](https://www.scribbr.com/statistics/statistical-significance/) is known as the critical value of _t_, or _t_*.
