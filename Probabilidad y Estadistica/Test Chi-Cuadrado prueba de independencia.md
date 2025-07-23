A **chi-square (Χ2) test of independence** is a [nonparametric](https://www.scribbr.com/statistics/statistical-tests/#nonparametric) [hypothesis test](https://www.scribbr.com/statistics/hypothesis-testing/). You can use it to test whether two [categorical variables](https://www.scribbr.com/methodology/types-of-variables/#quantitative-vs-categorical) are related to each other.

Definicion
No parametrico: Non-parametric tests don’t make as many assumptions about the data, and are useful when one or more of the common statistical assumptions are violated. However, the inferences they make aren’t as strong as with parametric tests.

`Imagine a city wants to encourage more of its residents to recycle their household waste.

`The city decides to test two interventions: an educational [flyer]pamphlet) or a phone call. They randomly select 300 households and [randomly assign] them to the flyer, phone call, or [control group] (no intervention). They’ll use the results of their experiment to decide which intervention to use for the whole city.

`The city plans to use a chi-square test of independence to test whether the proportion of households who recycle differs between the interventions.`

A chi-square (Χ2) test of independence is a type of Pearson’s [chi-square test](https://www.scribbr.com/statistics/chi-square-tests/). Pearson’s chi-square tests are nonparametric tests for categorical variables. They’re used to determine whether your data are [significantly](https://www.scribbr.com/statistics/statistical-significance/) different from what you expected.

You can use a chi-square test of independence to determine whether two categorical variables are related. If two [variables](https://www.scribbr.com/methodology/types-of-variables/) are related, the probability of one variable having a certain value is dependent on the value of the other variable.

When you want to perform a chi-square test of independence, the best way to organize your data is a type of **frequency distribution table** called a **contingency table**.
![[Pasted image 20250709190206.png]]

The hypotheses are two competing answers to the question “Are variable 1 and variable 2 related?”

- [Null hypothesis](https://www.scribbr.com/statistics/null-and-alternative-hypotheses/#definition) (_H_0): Variable 1 and variable 2 are **not related** in the population; The proportions of variable 1 are **the same** for different values of variable 2.
- [Alternative hypothesis](https://www.scribbr.com/statistics/null-and-alternative-hypotheses/#alternative) (_H_a): Variable 1 and  variable 2 are **related** in the population; The proportions of variable 1 are **not the same** for different values of  variable 2.

`- Null hypothesis (_H_0): Whether a household recycles and the type of intervention they receive are **not related** in the population; The proportion of households that recycle is **the same** for all interventions.
`- Alternative hypothesis (_H_a):  Whether a household recycles and the type of intervention they receive are **related** in the population; The proportion of households that recycle is **not the same** for all interventions.`

You can calculate the expected frequencies using the contingency table. The expected frequency for row _r_ and column _c_ is:
![[Pasted image 20250709190405.png]]
![[Pasted image 20250709190431.png]]
The expected frequencies are such that the proportion of households who recycle is the same for all interventions:

## When to use the chi-square test of independence

The following conditions are necessary if you want to perform a chi-square goodness of fit test:

1. You want to test a hypothesis about the relationship between **two** [**categorical variables**](https://www.scribbr.com/methodology/types-of-variables/#quantitative-vs-categorical) (binary, nominal, or ordinal).
    - Chi-square tests of independence are usually performed on binary or [nominal](https://www.scribbr.com/statistics/nominal-data/) variables. They are sometimes performed on [ordinal](https://www.scribbr.com/statistics/ordinal-data/) variables, although generally only on ordinal variables with fewer than five groups.
2. The **sample was** **random****l****y** **selected** from the [population](https://www.scribbr.com/methodology/population-vs-sample/).
3. There are a **minimum of five observations expected** in each combined group.

## How to perform the chi-square test of independence
### Step 1: Calculate the expected frequencies
![[Pasted image 20250709192012.png]]

### Step 2: Calculate chi-square

### Step 3: Find the critical chi-square value
```Python
from scipy.stats import chi2
chi2.ppf(0.95, df=2)
# 5.991464547107979
```
### Step 4: Compare the chi-square value to the critical value
Is the test statistic big enough to reject the null hypothesis? Compare it to the critical value to find out.
Χ2 = 9.79
Critical value = 5.99
The Χ2 value is greater than the critical value.

### Step 5: Decide whether to reject the null hypothesis
- If the Χ2 value is **greater** than the critical value, then the difference between the observed and expected distributions is statistically significant ([_p_](https://www.scribbr.com/statistics/p-value/) <  _α_).
    - The data allows you to [reject the null hypothesis](https://www.scribbr.com/statistics/hypothesis-testing/#step-4-decide-whether-to-reject-or-fail-to-reject-your-null-hypothesis) that the variables are unrelated and provides support for the [alternative hypothesis](https://www.scribbr.com/statistics/null-and-alternative-hypotheses/#alternative) that the variables are related.
- If the Χ2 value is **less** than the critical value, then the difference between the observed and expected distributions is not statistically significant (_p_ >  _α_).
    - The data doesn’t allow you to reject the null hypothesis that the variables are unrelated and doesn’t provide support for the alternative hypothesis that the variables are related.