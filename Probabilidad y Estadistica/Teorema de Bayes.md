==Permite calcular la probabilidad de un evento dado cierto conocimiento previo o evidencia, actualizando nuestras creencias a medida que obtenemos nueva información==
Sirve para calcular lo contrario de la prob condicional
P(A|B) = P(B|A) * P(A) / P(B) 
Donde:
- P(A|B) es la probabilidad del evento A dado que el evento B ha ocurrido (probabilidad posterior). 
- P(B|A) es la probabilidad del evento B dado que el evento A ha ocurrido (probabilidad condicional). 
- P(A) es la probabilidad inicial o probabilidad previa del evento A (probabilidad antes de considerar la evidencia B). 
- P(B) es la probabilidad del evento B (probabilidad de la evidencia total)

Supongamos que un laboratorio tiene tres máquinas (A, B y C) que producen envases. La máquina A produce el 40% de los envases y tiene un 2% de defectos. La máquina B produce el 30% con un 3% de defectos y la máquina C produce el 30% con un 5% de defectos

Si se selecciona un envase al azar y se descubre que está defectuoso, ¿Cuál es la probabilidad de que haya sido producido por la máquina A?
P(A) = 0.40
P(D | A) = 0.02
P(D) = 0.40 x 0.02 + 0.30 x 0.03 + 0.30 x 0.05 = 0.008 + 0.009 + 0.015 = 0.032 (probabilidad total de que sea defectuoso)

Entonces
P(A | D) = 0.4 x 0.02  / 0.032 = 25%
Por lo tanto, la probabilidad de que el envase defectuoso haya sido producido por la máquina A es del 25%
## ¿Cómo saber cuándo utilizar el teorema de Bayes?
Si necesita determinar la probabilidad de que algo ocurra dado que existe otra condición que puede influir en dicha ocurrencia, utilizaría el teorema de Bayes.