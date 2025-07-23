A Pearson’s **chi-square test** is a [[test estadístico]] for categorical data. It is used to determine whether your data are significantly different from what you expected. There are two types of Pearson’s chi-square tests:

- The [**chi-square goodness of fit test**](https://www.scribbr.com/statistics/chi-square-goodness-of-fit/) is used to test whether the frequency distribution of a categorical variable is different from your expectations.
- The [**chi-square test of independence**](https://www.scribbr.com/statistics/chi-square-test-of-independence/) is used to test whether two categorical variables are related to each other.

#### Definiciones:
Grado de libertad (Degrees of freedom): **Degrees of freedom**, often represented by _v_ or _df_, is the number of independent pieces of information used to calculate a [statistic](https://www.scribbr.com/statistics/test-statistic/). It’s calculated as the sample size minus the number of restrictions.
Degrees of freedom are normally reported in brackets beside the test statistic, alongside the results of the statistical test.
Nota: 
	**Although degrees of freedom are closely related to sample size, they’re not the same thing. There are always fewer degrees of freedom than the sample size.**
The number of independent pieces of information used to calculate the statistic is called the **degrees of freedom**. The degrees of freedom of a statistic depend on the sample size:

Nivel de significacia (Significance Level): The **significance level**, or alpha (α), is a value that the researcher sets in advance as the threshold for statistical significance. It is the maximum risk of making a false positive conclusion ([Type I error](https://www.scribbr.com/statistics/type-i-and-type-ii-errors/)) that you are willing to [accept](https://www.scribbr.com/commonly-confused-words/accept-vs-except/).

In a hypothesis test, the _p_ value is compared to the significance level to decide whether to reject the null hypothesis.

- If the _p_ value is **higher** than the significance level, the null hypothesis is not refuted, and the results are **not statistically significant**.
- If the _p_ value is **lower** than the significance level, the results are interpreted as refuting the null hypothesis and reported as **statistically significant**.

Usually, the significance level is set to 0.05 or 5%. That means your results must have a 5% or lower chance of occurring under the null hypothesis to be considered statistically significant.

#### [[Test Chi-Cuadrado prueba de bondad de ajuste]]
	
#### [[Test Chi-Cuadrado prueba de independencia]]
## Formula Chi Cuadrado
![[Pasted image 20250709161913.png]]
The larger the difference between the observations and the expectations (_O_ − _E_ in the equation), the bigger the chi-square will be.

##### Pasos para usar la formula Chi cuadrado
### Step 1: Create a table
Create a table with the observed and expected frequencies in two columns.
![[Pasted image 20250709162007.png]]
### Step 2: Calculate _O_ − _E_
Add a new column called “_O_ − _E_”. Subtract the expected frequencies from the observed frequency.
![[Pasted image 20250709162023.png]]

### Step 3: Calculate (_O_ − _E_)2
Add a new column called “(_O_ − _E_)2”. Square the values in the previous column.
![[Pasted image 20250709162042.png]]

### Step 4: Calculate (_O_ − _E_)2 / _E_

Add a final column called “(_O_ − _E_)² / _E_“. Divide the previous column by the expected frequencies.
![[Pasted image 20250709162053.png]]
### Step 5: Calculate Χ^2
Add up the values of the previous column. This is the chi-square test statistic (Χ2).
![[Pasted image 20250709162127.png]]

