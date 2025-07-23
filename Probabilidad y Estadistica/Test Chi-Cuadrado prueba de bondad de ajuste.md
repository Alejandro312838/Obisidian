Example: Chi-square goodness of fit test
	
	You’re hired by a dog food company to help them test three new dog food flavors.
	
	You recruit a  of 75 dogs and offer each dog a choice between the three flavors by placing bowls in front of them. You expect that the flavors will be equally popular among the dogs, with about 25 dogs choosing each flavor.
	
	Once you have your experimental results, you plan to use a chi-square goodness of fit test to figure out whether the distribution of the dogs’ flavor choices is significantly different from your expectations.
	
A chi-square (Χ2) goodness of fit test is a **goodness of fit** test for a [categorical variable](https://www.scribbr.com/methodology/types-of-variables/#quantitative-vs-categorical). Goodness of fit is a measure of how well a statistical model fits a set of observations.
- When goodness of fit is **high**, the values expected based on the model are **close to** the observed values.
- When goodness of fit is **low**, the values expected based on the model are **far from** the observed values.
The statistical models that are analyzed by chi-square goodness of fit tests are **distributions**.
The chi-square goodness of fit test is a [**hypothesis test**](https://www.scribbr.com/statistics/hypothesis-testing/). It allows you to [draw conclusions](https://www.scribbr.com/statistics/inferential-statistics/) about the distribution of a [population](https://www.scribbr.com/methodology/population-vs-sample/) based on a sample
Using the chi-square goodness of fit test, you can test whether the goodness of fit is “good enough” to conclude that the population follows the distribution.

	After weeks of hard work, your dog food experiment is complete and you compile your data in a table:

![[Pasted image 20250709161803.png]]

	To put it another way: You have a **sample** of 75 dogs, but what you really want to understand is the **population** of all dogs. Was this sample drawn from a population of dogs that choose the three flavors equally often?

## When to use the chi-square goodness of fit test

The following conditions are necessary if you want to perform a chi-square goodness of fit test:

1. You want to test a hypothesis about the distribution of **one** **categorical variable**. If your variable is [continuous](https://www.scribbr.com/methodology/types-of-variables/#quantitative-vs-categorical), you can convert it to a categorical variable by separating the observations into intervals. This process is known as data binning.
2. The **sample was** **randomly** **selected** from the [population](https://www.scribbr.com/methodology/population-vs-sample/).
3. There are a **minimum of five observations expected** in each group.
## How to perform the chi-square goodness of fit test
The chi-square statistic is a measure of goodness of fit, but on its own it doesn’t tell you much. For example, is Χ2 = 1.52 a low or high goodness of fit?
### Step 1: Calculate the expected frequencies
Sometimes, calculating the expected frequencies is the most difficult step. Think carefully about which expected values are most appropriate for your [null hypothesis](https://www.scribbr.com/statistics/null-and-alternative-hypotheses/#definition).
In general, you’ll need to multiply each group’s expected proportion by the total number of observations to get the expected frequencies.
### Step 2: Calculate chi-square
![[Pasted image 20250709162252.png]]

### Step 3: Find the critical chi-square value
Since there are three groups (Garlic Blast, Blueberry Delight, and Minty Munch), there are two degrees of freedom.
By convention, the significance level is usually .05.
```Python
from scipy.stats import chi2
chi2.ppf(0.95, df=2)
# 5.991464547107979
```

### Step 4: Compare the chi-square value to the critical value
Compare the chi-square value to the critical value to determine which is larger.
Χ2 = 1.52
Critical value = 5.99
The Χ2 value is less than the critical value

### Step 5: Decide whether the reject the null hypothesis
- If the Χ2 value is **greater** than the critical value, then the difference between the observed and expected distributions is statistically significant (_p_ <  _α_).
    - The data allows you to reject the null hypothesis and provides support for the alternative hypothesis.
- If the Χ2 value is **less** than the critical value, then the difference between the observed and expected distributions is not statistically significant (_p_ >  _α_).
    - The data doesn’t allow you to reject the null hypothesis and doesn’t provide support for the alternative hypothesis.


`The Χ2 value is less than the critical value. Therefore, you **should not reject** the null hypothesis that the dog population chooses the three flavors in equal proportions. There is no significant difference between the observed and expected flavor choice distribution (_p_ > .05). This suggests that the dog food flavors are equally popular in the dog population.`

`You report your findings back to the dog food company president. He decides not to eliminate the Garlic Blast and Minty Munch flavors based on your findings. The many dogs who love these flavors are very grateful!`
