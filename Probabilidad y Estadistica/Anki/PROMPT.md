Quiero que basado en la informacion que te ponga, hagas tarjetas de anki tipo pregunta-respuesta, definiciones ponlas en cartas separadas, formulas ponlas en la misma carta que su definicion, las imagenes (ej ![[Pasted image 20250709153653.png]]) dejalas tal cual como estan e incluyelas en las cartas, todo esto es relacionado a ciencia de datos asi que si ves necesario agregar una definicion importante que tenga que ver con esto hazlo, para los casos de "pasos para usar x" pon todos los pasos en la misma carta y de front algo como "cuales son los pasos para calcular chi cuadrado", debes de seguir el siguiente formato haciendo las cartas, los hiperlinks omitelos y eliminalos, para las partes que esten en ingles traducelas a español, pueden haber ejemplos esparcidos en las notas, por ejemplo "You recruit a  of 75 dogs and offer each dog a choice between the three flavors by placing bowls in front of them. You expect that the flavors will be equally popular among the dogs, with about 25 dogs choosing each flavor." ponlas donde creas que seas necesario pero NO hagas una carta para simplemente el ejemplo, tambien puede haber ejercicios, para estos vas a poner el problema en el front de la carta y la solucion en el back, te voy a ir dando el nombre de la nota para que puedas diferenciar donde empieza y termina cada una, este es el formato que debes de seguir, mas adelante te voy a pasar las notas asi que guarda este prompt en tu memoria, las cartas tienen un texto de "<!--ID: 1751763377336-->" ignoralo completamente, este se va a generar al momento de yo exportar las cartas
**¿Qué es la distribución binomial?** #flashcard
Es la **probabilidad de obtener un cierto número de éxitos en un número fijo de ensayos independientes, donde cada ensayo solo tiene dos posibles resultados (éxito o fracaso)**.  
Se utiliza para modelar situaciones donde se repite un experimento bajo las mismas condiciones varias veces y se cuenta el número de veces que ocurre un evento específico.
**Características:**
- **Independencia de los ensayos:** los resultados de un ensayo no afectan a los demás (ej. lanzamiento de monedas).
- **Probabilidad de éxito constante:** la probabilidad de éxito (p) es igual en cada ensayo.
**Ejemplo:**
- Calcular la probabilidad de obtener exactamente 3 caras en 5 lanzamientos de una moneda justa.  
    ![[Pasted image 20250705182004.png]]  
    ![[Pasted image 20250705182105.png]]
**Media y varianza:**
- Media:  
    ![[Pasted image 20250705184839.png]]
- Varianza:  
    ![[Pasted image 20250705184905.png]]
<!--ID: 1751763377336-->



**¿Qué es la distribución de Poisson?** #flashcard
Es una **distribución de probabilidad discreta que describe la probabilidad de que ocurra un cierto número de eventos en un intervalo de tiempo o espacio dado, asumiendo que estos eventos ocurren con una tasa promedio constante y de forma independiente**.
**Características:**
- Un solo parámetro λ (lambda), que es la tasa promedio.
- Modela **eventos raros** o poco frecuentes.
- Asume **independencia** entre eventos.
**Ejemplo de cuándo usarla:**
1. Eventos ocurren al azar e independientemente.
2. Sabes el número promedio de eventos (λ) en un intervalo fijo.
![[Pasted image 20250705182437.png]]
**Nota:** En Poisson, **media y varianza son iguales a λ**.
<!--ID: 1751763368547-->



**¿Qué es la distribución de Bernoulli?** #flashcard
Representa una variable aleatoria discreta con **dos resultados mutuamente excluyentes (éxito o no éxito)**.  
Solo aplica para **un solo experimento**.  
Si haces varios, debes usar la binomial.
**Ejemplo:**
- Tirar un dado: si definimos éxito como obtener un 6, entonces “no éxito” es obtener 1, 2, 3, 4 o 5.
**Probabilidades:**
- P(X=1) = p (éxito)
- P(X=0) = 1-p (fracaso)
**Media y varianza:**
- E(X) = p
- Var(X) = p(1-p)
<!--ID: 1751763368594-->
