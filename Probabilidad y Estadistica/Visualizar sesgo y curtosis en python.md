Uno de los mejores medios visuales para ver la forma y, por tanto, la asimetría y la curtosis de las distribuciones es un **gráfico de estimación de la densidad del kernel (KDE)**. Se puede utilizar a través de Seaborn:
```python
import matplotlib.pyplot as plt

sns.kdeplot(diamond_prices)

plt.title("KDE plot of diamond prices")
plt.xlabel("Price ($)")
```
![[Pasted image 20250704181138.png]]

##### Cuando la linea KDE sea muy irregular
bw_adjust por defecto es 1
```python
sns.kdeplot(diamonds["carat"], bw_adjust=3, color="red")
```

##### Cuando usas KDE superpuesto en un histograma
kdw_kws controla la sensibilidad del KDE
```python
ax = sns.histplot(
   diamonds["carat"],
   kde=True,
   kde_kws=dict(bw_adjust=3),
   bins=25,
)
```
