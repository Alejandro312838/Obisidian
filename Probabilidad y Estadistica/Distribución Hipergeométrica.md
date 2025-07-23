La distribución hipergeométrica es un ==modelo estadístico discreto que se utiliza para calcular la probabilidad de obtener un número específico de éxitos en una muestra sin reemplazo de una población finita==. En otras palabras, describe la probabilidad de un número determinado de éxitos en un número fijo de ensayos, donde la probabilidad de éxito no es la misma en cada ensayo.
##### Características
**Muestreo sin reemplazo:**
A diferencia de la distribución binomial, en la hipergeométrica no se devuelve el elemento extraído a la población, lo que significa que la probabilidad de éxito cambia en cada ensayo. 
- **Población finita:**
    La distribución se aplica a situaciones donde se trabaja con un número limitado de elementos en la población. 
- **Dos resultados posibles:**
    Cada ensayo tiene dos resultados posibles, generalmente etiquetados como "éxito" o "fracaso".
Formula:
![[Pasted image 20250705183431.png]]

La media es:
μ = n * (k/N)
Donde: 
- **n:** Es el número de ensayos o el tamaño de la muestra.
- **k:** Es el número de éxitos en la población.
- **N:** Es el tamaño de la población.

La varianza es:
![[Pasted image 20250705184431.png]]
Donde: 
- **n:** Es el número de ensayos o el tamaño de la muestra.
- **k:** Es el número de éxitos en la población.
- **N:** Es el tamaño de la población.

Ejemplo:
De cada 20 piezas fabricadas por una máquina, hay 2 que son defectuosas. Para realizar un   control de calidad, se observan 15 elementos y se rechaza el lote si hay alguna que sea defectuoso. Vamos a calcular la probabilidad de que el lote sea rechazado.
![[Pasted image 20250705183707.png]]

==Cuando N es muy grande, como criterio se suele considerar N > 10n, la distribución hipergeométrica se puede aproximar por la binomial B( n, p ) con p = k/N.==
