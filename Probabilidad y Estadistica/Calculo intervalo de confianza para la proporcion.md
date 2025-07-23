**Como la proporción p de la población es desconocida, se aproxima por la de la muestra siempre que n>100.**

Es para datos categoricos

**¿Cómo sabe que está ante un problema de proporción?** En primer lugar, la **distribución subyacente tiene una variable aleatoria binaria y, por tanto, es una** distribución binomial. (No se menciona la media o el promedio). Si _X_ es una variable aleatoria binomial, entonces _X_ ~ _B_(_n_, _p_) donde _n_ es el número de ensayos y _p_ es la probabilidad de acierto Para formar una proporción de la muestra, tome _X_, la variable aleatoria para el número de aciertos y divídala por _n_, el número de ensayos (o el tamaño de la muestra). La variable aleatoria _P′_ (léase "P prima") es la proporción de la muestra,
![[Pasted image 20250716184741.png]]


Formula distribucion estandar
![[Pasted image 20250716184514.png]]

Por lo tanto el intervalo de confianza para la proporcion
![[Pasted image 20250716184532.png]]
Las **proporciones muestrales _p′_ y _q′_ son estimaciones de las proporciones poblacionales desconocidas _p_ y _q_**. Se utilizan las proporciones estimadas _p′_ y _q′_ porque _p_ y _q_ no se conocen.

(_p′_ y _q′_  pertenecen a la muestra y _p_ y _q_ a la poblacion)

## Formula para el intervalo de confianza de proporciones de MUESTRAS
![[Pasted image 20250716192653.png]]

## Ejercicio
Problema:
Supongamos que se contrata a una compañía de estudios de mercado para que estime el porcentaje de adultos que viven en una gran ciudad y que tienen teléfonos móviles. Se encuestan quinientos residentes adultos seleccionados al azar en esta ciudad para determinar si tienen teléfonos móviles. De las 500 personas incluidas en la muestra, 421 respondieron que sí: tienen teléfonos móviles. Utilizando un nivel de confianza del 95 %, calcule una estimación del intervalo de confianza para la verdadera proporción de residentes adultos de esta ciudad que tienen teléfonos móviles.

Solucion:
Supongamos que _X_ = el número de personas de la muestra que tienen teléfonos móviles. _X_ es binomial: la variable aleatoria es binaria, la gente o tiene un teléfono móvil o no lo tiene.

Para calcular el intervalo de confianza, debemos hallar _p′_, _q′_.

n = 500
_x_ = número de aciertos en la muestra = 421
Calculando p:
![[Pasted image 20250716185101.png]]
_p′_ = 0,842 es la proporción de la muestra; es la estimación puntual de la proporción de la población.
_q′_ = 1 – _p′_ = 1 – 0,842 = 0,158
Como el nivel de confianza solicitado es _CL_ = 0,95, entonces _α_ = 1 - _CL_ = 1 - 0,95 = 0,05 (α/2) = 0,025.
z(0.025) = 1.96 Este se obtiene a traves de las tablas de valor z

Sustituyendo en la formula:
![[Pasted image 20250716185206.png]]
Sustituyendo los valores anteriores encontramos que el intervalo de confianza es:
0,810 ≤ p ≤ 0,874
### Interpretación
Estimamos con el 95 % de confianza que entre el 81 % y el 87,4 % de todos los residentes adultos de esta ciudad tienen teléfonos móviles.
