La distribución geométrica es un ==modelo de probabilidad que describe el número de intentos necesarios para obtener el primer éxito en una serie de experimentos de Bernoulli independientes, donde cada experimento tiene la misma probabilidad de éxito==. En otras palabras, calcula la probabilidad de tener que realizar un cierto número de intentos antes de obtener el primer resultado deseado
**Sin memoria:**
La probabilidad de éxito en el siguiente intento no depende de cuántos intentos fallidos se hayan realizado anteriormente.
**Fórmula:**
La función de probabilidad de masa (PMF) de la distribución geométrica es:
P(X=k) = (1-p)^(k-1) * p
Donde: 
- `P(X=k)` es la probabilidad de obtener el primer éxito en el intento `k`.
- `p` es la probabilidad de éxito en un solo intento.
- `k` es el número de intentos hasta obtener el primer éxito (k=1, 2, 3, ...).
La función de masa de probabilidad se define como la probabilidad de que una variable aleatoria discreta, X, sea exactamente igual a un valor, x.

función de distribución acumulada (FDC) es:
- **Distribución geométrica CDF:** P(X ≤ x) = 1 - (1 - p)^x
La función de distribución acumulativa de una variable aleatoria, X, que se evalúa en un punto, x, se puede definir como la probabilidad de que X tome un valor menor o igual a x.

La media de una distribucion geometrica es
![[Pasted image 20250705183207.png]]
donde p =  es la probabilidad de éxito en un solo intento.

La varianza es de una distribucion geometrica es:
![[Pasted image 20250705183224.png]]
donde p =  es la probabilidad de éxito en un solo intento.

Ejemplos de aplicación:
- **Control de calidad:**
    Calcular la probabilidad de encontrar el primer producto defectuoso después de inspeccionar un cierto número de unidades.
- **Deportes:**
    Determinar la probabilidad de que un jugador enceste su primer tiro libre después de varios intentos fallidos.