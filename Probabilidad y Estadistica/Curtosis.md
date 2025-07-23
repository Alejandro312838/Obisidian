La curtosis se refiere a la medida de la forma de una distribución en comparación con la distribución normal, también conocida como campana de Gauss.
la curtosis nos permite comprender mejor cómo se distribuyen los datos alrededor de la media y si hay valores atípicos.
La información proporcionada puede ser útil en diferentes situaciones. Por ejemplo, en finanzas, la curtosis puede ayudarnos a comprender la volatilidad de los precios de las acciones. Una curtosis alta podría indicar un mayor riesgo y la posibilidad de eventos extremos, mientras que una curtosis baja podría señalar una mayor estabilidad en los precios.
###### Tipos de curtosis
1. **Distribución mesocúrtica** (curtosis = 3, exceso de curtosis = 0): distribución normal perfecta o muy próxima a ella.
2. **Distribución leptocúrtica** (curtosis > 3, exceso de curtosis > 0): pico agudo, colas pesadas
3. **Distribución platicúrtica** (curtosis < 3, exceso de curtosis < 0): pico plano, colas ligeras
![[Pasted image 20250704180828.png]]
![[Pasted image 20250704180859.png]]

##### Calculo en python

```python
from scipy.stats import kurtosis

kurtosis(diamond_prices)
```

Usando pandas
Para series panda
```python
diamond_prices.kurt()
```

Para dataframes
```python
diamonds.select_dtypes(include="number").kurtosis()
```