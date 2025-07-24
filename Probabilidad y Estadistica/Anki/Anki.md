TARGET DECK: Intellectual Greed

**¿Qué es la prueba t de Student para datos independientes?** #flashcard
Es una **prueba estadística utilizada para comparar las medias de dos grupos y determinar si existe una diferencia significativa entre ellas**.  
Se aplica cuando:
- Se desconoce la desviación estándar poblacional.
- El tamaño de muestra es pequeño.
- Las muestras son **independientes**.
    
<!--ID: 1753324830632-->


---

**¿Qué es el Error Estándar de la Diferencia entre Medias (SED) y cual es su formula?** #flashcard
Es una medida que cuantifica la variabilidad en la diferencia entre dos medias muestrales.  
Se usa como base para calcular el estadístico t en la prueba de dos muestras.  
![[Pasted image 20250723200509.png]]
<!--ID: 1753324830651-->


---

**¿Qué es el Error Estándar de la Diferencia entre Medias estimado a partir de muestras y cual es su formula?** #flashcard
Cuando no se conoce la varianza poblacional, se usa una estimación a partir de los datos muestrales.  
![[Pasted image 20250723200556.png]]
<!--ID: 1753324830658-->


---

**¿Cuál es la fórmula de la prueba t para datos independientes?** #flashcard
La fórmula de la prueba t para comparar dos medias con muestras independientes es:  
![[Pasted image 20250723200645.png]]  
**Criterio de decisión:**
- Si |t observado| > t crítico → **Rechazas Ho**
- Si |t observado| ≤ t crítico → **No rechazas Ho**
    
<!--ID: 1753324830665-->


---

**Ejemplo de aplicación de la prueba t para datos independientes** #flashcard
![[Pasted image 20250723200753.png]]
<!--ID: 1753324830672-->


**¿Qué son las pruebas paramétricas?** #flashcard
Las **pruebas paramétricas** son herramientas estadísticas utilizadas para analizar los factores de una población bajo ciertos supuestos.  
Requieren que la muestra siga una **distribución específica** (normal en la mayoría de los casos) y que las variables sean **numéricas**.  
Estas pruebas son más fiables cuanto mayor es el tamaño de la muestra.
<!--ID: 1753324830678-->


---

**¿Cuáles son las condiciones que deben cumplir las pruebas paramétricas?** #flashcard

1. **Normalidad:** Las observaciones deben ajustarse a una distribución normal (se puede comprobar con pruebas de bondad de ajuste).
2. **Homocedasticidad:** Las varianzas de los grupos deben ser homogéneas.
3. **Independencia de errores:** Los errores deben ser independientes; esto sucede cuando los sujetos se asignan de forma aleatoria y están distribuidos normalmente en el grupo.
    
<!--ID: 1753324830685-->


---

**¿Cuáles son las ventajas de las pruebas paramétricas?** #flashcard
- Son más eficientes.
- Son sensibles a las características de los datos.
- La probabilidad de errores es muy baja.
- Los cálculos probabilísticos son muy exactos.
    
<!--ID: 1753324830691-->


---
**¿Cuáles son las desventajas de las pruebas paramétricas?** #flashcard
- Los cálculos pueden ser complejos.
- Solo se pueden aplicar a ciertos tipos de datos observables (numéricos y con ciertas propiedades).
    
<!--ID: 1753324830698-->


---

**¿Cuáles son los tipos de pruebas paramétricas?** #flashcard
- Prueba del valor Z de la distribución normal
- Prueba T de Student para datos relacionados (muestras dependientes)
- Prueba T de Student para datos independientes (muestras independientes)
- Prueba T de Student-Welch para dos muestras independientes con varianzas no homogéneas
- Prueba de Ji Cuadrada de Bartlett para demostrar la homogeneidad de varianzas
- Prueba F (análisis de varianza o ANOVA)
<!--ID: 1753324830704-->



**¿Qué es la Máxima Verosimilitud (MLE)?** #flashcard
Es un **método estadístico utilizado para estimar los parámetros de un modelo**.  
Busca los valores de los parámetros que hacen **más probable haber observado los datos que tenemos**.  
Se usa en estadística, aprendizaje automático, bioinformática, entre otros.
<!--ID: 1752806165187-->


---

**¿Cuál es el objetivo del método de máxima verosimilitud (MLE)?** #flashcard
Encontrar los **valores de los parámetros que maximizan la función de verosimilitud**, es decir, los que hacen que los datos observados sean más probables.
<!--ID: 1752806165245-->


---

**¿Cuál es la condición necesaria para usar la MLE?** #flashcard
**Siempre debe asumirse que los datos provienen de una distribución definida** (normal, binomial, exponencial, etc.).  
Sin esta suposición, **no puede aplicarse la MLE tradicional**.
<!--ID: 1752806165255-->


---

**¿Qué es la función de verosimilitud?** #flashcard
Es una **función que describe la probabilidad de observar los datos que tenemos dado un conjunto específico de valores para los parámetros**.
![[Pasted image 20250717164731.png]]
En este caso debemos de calcular los parametros que nos darian la distribucion azul pues es la que mejor explica los datos
<!--ID: 1752806165264-->


---

**¿Cuáles son los pasos para encontrar la función de verosimilitud?** #flashcard
1. **Identificar la distribución de la muestra**
2. **Escribir la función de densidad o probabilidad** para una observación f(xi ; θ) donde θ es el parametro
3. **Construir la función de verosimilitud**  
     ![[Pasted image 20250717202214.png]]
     = f(x1 ; θ) x ... x f(xn ; θ)
4. **Tomar logaritmo natural** (log-verosimilitud):  
      ![[Pasted image 20250717202315.png]]
5. **Derivar con respecto al parametro θ e igualar a cero:**  
    ![[Pasted image 20250717202413.png]]
6. **Verificar que es un máximo** (segunda derivada o análisis gráfico)
    Si el resultado es negativo entonces si es un maximo
<!--ID: 1752806165272-->


---

**¿Qué interpreta la estimación de máxima verosimilitud?** #flashcard
Los valores de los parámetros que **mejor explican los datos observados**, según el modelo estadístico asumido.
<!--ID: 1752806165280-->


---

**¿Qué ocurre si no se conoce la distribución de los datos?** #flashcard
No se puede usar MLE tradicional. En ese caso, se puede:
- Usar una distribución aproximada (modelo paramétrico).
- Usar métodos no paramétricos (ej. histogramas, estimadores kernel, bootstrap).
- Usar modelos semi-paramétricos (parte del modelo conocida y parte no).
    
<!--ID: 1752806165288-->


---

**¿Cuál es la MLE para la media de una distribución normal con varianza conocida?** #flashcard
La estimación de máxima verosimilitud es el **promedio muestral**:  
μ^=1n∑xi\hat{\mu} = \frac{1}{n} \sum x_i
<!--ID: 1752806165296-->


---

**¿Cuál es la MLE para el parámetro λ de una distribución exponencial?** #flashcard 
λ^=n∑xi=1xˉ\hat{\lambda} = \frac{n}{\sum x_i} = \frac{1}{\bar{x}}
<!--ID: 1752806165304-->


---

**¿Qué significa que la MLE tenga una "forma fija"?** #flashcard
La **fórmula del estimador no cambia** para una misma distribución.  
Lo que cambia entre muestras es **el valor numérico** del estimador, **no su forma**.
<!--ID: 1752806165312-->


---


**¿Qué es la estimación de parámetros?** #flashcard
Es un **proceso estadístico que busca determinar el valor de características desconocidas (parámetros) de una población utilizando datos de una muestra**.  
Puede hacerse mediante:
- **Estimación puntual:** se obtiene un único valor.
- **Estimación por intervalos:** se obtiene un rango de valores con cierto nivel de confianza.
    
<!--ID: 1752716362655-->


---
**¿Qué es un parámetro?** #flashcard
Es una **característica numérica de una población**, como la media, la desviación estándar o la proporción.
<!--ID: 1752716362690-->


---

**¿Qué es un estimador?** #flashcard
Es un **valor calculado a partir de los datos muestrales** que proporciona información sobre un parámetro.  
Ejemplos:
- Media muestral → estima la media poblacional.
- Proporción observada → estima la proporción poblacional.
    
<!--ID: 1752716362701-->


---

**¿Qué es una estimación?** #flashcard
Es el **valor numérico obtenido al aplicar un estimador a los datos de la muestra**.
<!--ID: 1752716362709-->


---

---

**¿Qué es un intervalo de confianza?** #flashcard
Es un **rango de valores que, con un cierto nivel de confianza, se espera que contenga el verdadero valor del parámetro poblacional**.
<!--ID: 1752716362717-->


---

**¿Qué es el nivel de confianza?** #flashcard
Es la **probabilidad de que el intervalo de confianza contenga el verdadero valor del parámetro**.
<!--ID: 1752716362726-->


---

**¿Qué es el error estándar de la media?** #flashcard
![[Pasted image 20250716180109.png]]
<!--ID: 1752716362733-->


---

**¿Qué es un estadístico?** #flashcard
Se refiere a **medidas obtenidas a partir de una muestra**.
<!--ID: 1752716362743-->


---

**¿Qué estadisticos se pueden estimar a partir de una muestra?** #flashcard
![[Pasted image 20250716175710.png]]  
_El símbolo con gorrito indica que fue estimado a través de una muestra._
<!--ID: 1752716363048-->


---

**¿Qué es la estimación puntual?** #flashcard
Es un **tipo de estimación donde se calcula un único valor para el parámetro poblacional**.  
Ejemplo: usar la media muestral como estimación de la media poblacional.
<!--ID: 1752716363058-->


---

**¿Qué es la estimación por intervalos?** #flashcard
Es un **tipo de estimación donde se calcula un rango de valores que probablemente contenga el verdadero valor del parámetro**, expresado con un nivel de confianza.  
Ejemplo: intervalo de confianza del 95% para la media poblacional.
<!--ID: 1752716363067-->


---

**¿Por qué es preferible la estimación por intervalos sobre la puntual?** #flashcard
![[Pasted image 20250716180302.png]]  
Porque diferentes muestras pueden producir diferentes medias, pero la mayoría de sus intervalos de confianza contendrán la media poblacional verdadera.
<!--ID: 1752716363077-->


---

**¿Cuál es la fórmula para calcular el intervalo de confianza para la media?** #flashcard
![[Pasted image 20250716180531.png]]
![[Pasted image 20250716180737.png]]
<!--ID: 1752716363085-->


---


---

**¿Cuál es la fórmula del intervalo de confianza de la media en MUESTRAS?** #flashcard
![[Pasted image 20250716192557.png]]  
Donde:
- s = desviación estándar
- n = tamaño de la muestra
    
<!--ID: 1752716363093-->


---

**¿Cuál es el intervalo de confianza en el siguiente problema?** Se pretende estimar la media de frecuencia cardiaca para cierta población. Se encontró que el número promedio de latidos del corazón/minuto para 49 personas era de 90.Considere que esos 49 pacientes constituyen una muestra aleatoria y que la población sigue una distribución normal, con una desviación estándar de 10. #flashcard
**Problema:**
![[Pasted image 20250716181045.png]]
**Solución:**  
![[Pasted image 20250716181055.png]]  
_Valores de Z como Z(90%) y Z(95%) se obtienen con una tabla de valores Z._
<!--ID: 1752716363101-->


---

**¿Qué es un intervalo de confianza para una proporción?** #flashcard
Es una **estimación para la proporción poblacional cuando se trabaja con variables categóricas**, especialmente cuando la variable sigue una distribución binomial.  
Se usa cuando no se menciona la media o promedio.
<!--ID: 1752716363113-->


---

**¿Cómo se forma una proporción muestral en un problema binomial?** #flashcard
Si _X_ es el número de aciertos y _n_ el tamaño de la muestra:  
 _p′_ = _X_ / _n_  
![[Pasted image 20250716184741.png]]
<!--ID: 1752716363124-->


---

**¿Cuál es la fórmula de la desviación estándar para proporciones?** #flashcard
![[Pasted image 20250716184514.png]]
<!--ID: 1752716363132-->


---

**¿Cuál es la fórmula para el intervalo de confianza de una proporción?** #flashcard
![[Pasted image 20250716184532.png]]  
Nota: _p′_ y _q′_ son estimaciones de las proporciones poblacionales _p_ y _q_.
<!--ID: 1752716363142-->


---

**¿Cuál es la fórmula para el intervalo de confianza de proporciones en muestras?** #flashcard
![[Pasted image 20250716192653.png]]
<!--ID: 1752716363152-->


---

**¿Cuál es el intervalo de confianza para este problema de proporciones?** Se desea estimar el porcentaje de adultos en una ciudad que tienen teléfonos móviles. De 500 personas encuestadas, 421 tienen teléfono. Calcule el intervalo de confianza al 95%. #flashcard
**Problema:**  
Se desea estimar el porcentaje de adultos en una ciudad que tienen teléfonos móviles.  
De 500 personas encuestadas, 421 tienen teléfono. Calcule el intervalo de confianza al 95%.
**Solución:**
- n = 500
- x = 421
- p′ = 421/500 = 0,842
- q′ = 1 - 0,842 = 0,158
- z(0.025) = 1.96  
    ![[Pasted image 20250716185101.png]]  
    ![[Pasted image 20250716185206.png]]  
    **Resultado:**  
    0,810 ≤ p ≤ 0,874  
    **Interpretación:**  
    Con un 95% de confianza, entre el 81% y el 87,4% de los adultos tienen teléfono móvil.
    
<!--ID: 1752716363161-->


---

**¿Cuál es la fórmula de el margen de error "E"?** #flashcard 
![[Pasted image 20250716191331.png]]  
Donde:
- E = margen de error
- p y q = proporciones
- z = valor Z de confianza
    
<!--ID: 1752716363169-->


---

**¿Cuál es la fórmula para estimar el tamaño de muestra?** #flashcard
![[Pasted image 20250716191421.png]]  
o también  
![[Pasted image 20250716191112.png]]
<!--ID: 1752716363178-->


---

**Ejercicio: ¿Cuál es el tamaño muestral necesario si el margen de error es 3% y el nivel de confianza es 95%?** #flashcard
**Problema:**  
Estimar el tamaño muestral necesario para una encuesta presidencial nacional si el margen de error deseado es de 3%. Asumir 95% de confianza.
**Solución:**
- z = 1.96 (para 95% de confianza)
- Sustituyendo en la fórmula:  
    ![[Pasted image 20250716191514.png]]
    
<!--ID: 1752716363191-->



**¿Qué es el muestreo aleatorio simple?** #flashcard
Es un **método para seleccionar una muestra de una población donde cada individuo tiene la misma probabilidad de ser elegido**.  
Es una técnica fundamental en estadística para obtener una muestra representativa de la población y realizar inferencias sobre ella.


**¿Cuáles son las ventajas del muestreo aleatorio simple?** #flashcard
- **Representatividad:** Permite obtener una muestra que refleja las características de la población.
- **Simplicidad:** Es relativamente fácil de entender y aplicar.
- **Generalización:** Permite inferir resultados a toda la población con un margen de error controlado.  
    Además, al usar aleatorización, cualquier investigación basada en esta muestra tendrá alta **validez interna y externa**, con menor riesgo de sesgos como el **sesgo de muestreo** o el **sesgo de selección**.
    
<!--ID: 1752545416174-->


---

**¿Cuáles son las desventajas del muestreo aleatorio simple?** #flashcard

- **Requiere un listado completo de la población**, lo cual puede ser complicado en poblaciones grandes.
- **Costos y tiempo elevados** en poblaciones extensas.
- **No siempre es ideal** si se necesitan resultados específicos sobre subgrupos de la población.
    
<!--ID: 1752545416214-->


---

**¿Cuáles son los pasos para realizar un muestreo aleatorio simple?** #flashcard
1. **Definir la población:**  
    Determinar el grupo total del cual se desea obtener la muestra, asegurando acceso a todos sus miembros.
2. **Decidir el tamaño de la muestra:**
    - Tamaños más grandes brindan mayor certeza estadística pero aumentan costos.
    - Se puede usar un intervalo de confianza (0.05) y un nivel de confianza (0.95), con un valor de desviación estándar estimado (por ejemplo, 0.5), o una calculadora de tamaño muestral.
3. **Seleccionar aleatoriamente la muestra:**
    - **Método de lotería:** “sacar papelitos de un sombrero” o usar un programa que simule esta acción.
    - **Método de números aleatorios:** Asignar un número a cada individuo y usar un generador de números aleatorios (o tablas) para seleccionar los que formarán la muestra.
    - Ejemplo: usar `RAND` en Excel.
4. **Recolectar datos de la muestra:**  
    Es crucial que todos los individuos seleccionados participen efectivamente. Si ciertos grupos, como los jóvenes, no participan, esto podría sesgar los resultados y afectar la validez del estudio.
    
<!--ID: 1752545416224-->


---

**¿Qué son las técnicas de muestreo?** #flashcard
Son **métodos para seleccionar una parte representativa de una población para su estudio**, permitiendo inferir conclusiones sobre toda la población.
<!--ID: 1752532227254-->


---

**¿Cómo se dividen principalmente las técnicas de muestreo?** #flashcard
En dos grandes tipos:
- **Muestreo probabilístico (aleatorio)**
- **Muestreo no probabilístico**
    
<!--ID: 1752532227267-->


---

**¿Qué caracteriza al muestreo probabilístico o aleatorio?** #flashcard
Que **todos los individuos tienen la misma probabilidad de ser seleccionados**, eliminando sesgos y asegurando rigor metodológico. Es el más confiable.  
Ejemplo: sacar bolitas numeradas de una urna donde cada una tiene igual oportunidad.
<!--ID: 1752532227282-->


---

**¿Qué es el muestreo aleatorio simple?** #flashcard
Cada individuo tiene **la misma probabilidad de ser elegido**. Es el método más sencillo y común, pero poco eficiente en poblaciones muy grandes.  
Ejemplo: poner los nombres de todos los estudiantes de una escuela en un sombrero y sacar 50 al azar.
<!--ID: 1752532227294-->


---

**¿Qué es el muestreo sistemático?** #flashcard
Se enumeran todos los individuos, se elige el primero **aleatoriamente**, y los demás se seleccionan **periódicamente** (por ejemplo, cada 10).  
Puede ser problemático si hay ciclos en la población.  
Ejemplo: en una lista de 1000 clientes ordenada alfabéticamente, elegir al azar el cliente número 5 y luego seleccionar cada décimo cliente (15, 25, 35, etc.).
<!--ID: 1752532227306-->


---

**¿Qué es el muestreo estratificado?** #flashcard
La población se **divide en estratos homogéneos** según características relevantes, y luego se selecciona **aleatoriamente una muestra proporcional** de cada estrato.  
Aumenta la representatividad.  
Ejemplo: dividir a los empleados de una empresa por departamento y tomar un porcentaje de cada departamento para asegurar representación.
<!--ID: 1752532227316-->


---

**¿Qué es el muestreo por conglomerados?** #flashcard
Se eligen **grupos o conglomerados completos aleatoriamente**, no individuos.  
Ejemplo: en vez de elegir estudiantes individuales de todo un país, se seleccionan escuelas completas al azar y luego se encuesta a todos sus estudiantes.
<!--ID: 1752532227325-->


---

**¿Qué caracteriza al muestreo no probabilístico?** #flashcard
No se basa en igualdad de probabilidades. Se usan **criterios subjetivos o prácticos** para seleccionar la muestra.  
Tiene menor representatividad y confiabilidad, pero es útil ante restricciones de tiempo o costo, o para estudios exploratorios.  
Ejemplo: entrevistar a los primeros 20 clientes que entran a una tienda un lunes por la mañana.
<!--ID: 1752532227333-->


---

**¿Qué es el muestreo por cuotas?** #flashcard
Se fijan características o condiciones que debe cumplir la muestra, y se selecciona un número de elementos que las cumpla.  
Muy usado en encuestas de opinión.  
Ejemplo: en una encuesta política, decidir que el 50% sean hombres y el 50% mujeres, y luego ir reclutando hasta cumplir esas proporciones.
<!--ID: 1752532227343-->


---

**¿Qué es el muestreo intencional?** #flashcard
Se eligen **intencionadamente** individuos o grupos que se consideran representativos. Requiere gran conocimiento de la población.  
Frecuente en encuestas de intención de voto.  
Ejemplo: un investigador elige entrevistar líderes comunitarios porque cree que representan la opinión de todo el vecindario.
<!--ID: 1752532227351-->


---

**¿Qué es el muestreo en cadena?** #flashcard
Se seleccionan algunos individuos iniciales, y estos **remiten o conectan con otros** para ir ampliando la muestra.  
Se usa con poblaciones marginales o difíciles de acceder (delincuencia, enfermedades).  
Ejemplo: entrevistar a un usuario de drogas que luego presenta a otros consumidores para continuar el estudio.
<!--ID: 1752532227359-->


---

**¿Qué es el muestreo discrecional?** #flashcard
El investigador **elige deliberadamente** los elementos que considera más adecuados para el estudio.  
Totalmente dependiente del criterio del investigador.  
Ejemplo: un experto en historia selecciona documentos que él considera los más relevantes para analizar un periodo.
<!--ID: 1752532227369-->


---

Si quieres, también puedo darte un **cuadro comparativo final** entre probabilístico y no probabilístico con ejemplos paralelos. ¡Solo dime!

**¿Qué es la distribución t de Student?** #flashcard
La **distribución t de Student** es un tipo de distribución normal usada cuando el tamaño de muestra es pequeño y la varianza poblacional es desconocida.
- Tiene forma de campana (bell shape), similar a la normal, pero con colas más gruesas, lo que refleja mayor incertidumbre.
    
<!--ID: 1752531513142-->


---

**¿Cuándo se usa la distribución t de Student?** #flashcard
Se usa cuando:
- Los datos están **aproximadamente normalmente distribuidos** (siguen forma de campana).
- La **varianza poblacional es desconocida**, por lo que se estima con la muestra.
<!--ID: 1752531513153-->


---

**¿Cómo cambia la distribución t con los grados de libertad?** #flashcard
A medida que los **grados de libertad** (`df = n - 1`) aumentan:
- La distribución t se va pareciendo cada vez más a la **distribución normal estándar (z)**.
- Con más de **30 grados de libertad**, la t y la z son prácticamente iguales, y se puede usar la z.
    
<!--ID: 1752531513160-->


---

**¿Por qué la distribución z es preferible a la t cuando se puede?** #flashcard
- La **distribución z** tiene **varianza conocida**, por lo que hace estimaciones más precisas.
- La **distribución t** usa una varianza aproximada (basada en los grados de libertad), lo que introduce mayor incertidumbre.  
    Por eso, se usa t solo cuando la varianza poblacional es desconocida y el tamaño de muestra es pequeño.
    
<!--ID: 1752531513171-->


---

**¿Qué es un valor t o t-score?** #flashcard
Un **t-score** indica cuántas **desviaciones estándar** se encuentra un valor respecto a la media en una distribución t.  
Se puede:
- Consultar en tablas t
- Calcular con herramientas en línea
    
<!--ID: 1752531513182-->


---

**¿Para qué se usan los valores t?** #flashcard
1. Para determinar los **límites superior e inferior** de un intervalo de confianza.
2. Para calcular el **p-valor** en pruebas estadísticas como t-tests y regresión.
    
<!--ID: 1752531513193-->


---

**¿Qué es el t crítico o t?** #flashcard
El t crítico (`*t`) es el valor t que define el límite de una región crítica:
- Se usa para construir intervalos de confianza.
- O para comparar contra un t calculado y decidir si el resultado es estadísticamente significativo (relacionado con el p-valor).
    
<!--ID: 1752531513201-->


---
**¿Qué es la distribución F?** #flashcard
La **distribución F**, también conocida como distribución de **Fisher-Snedecor**, se usa para **comparar varianzas entre poblaciones** y evaluar si la diferencia observada entre dos grupos se debe al azar o a factores significativos.
- Permite analizar cuán **dispersos** están los valores de dos conjuntos de datos respecto a sus medias.
    
<!--ID: 1752531231499-->


---

**¿Cómo se define formalmente la distribución F?** #flashcard
Si
- `U` y `V` son variables aleatorias independientes que siguen distribuciones Chi-Cuadrado con `d1` y `d2` grados de libertad respectivamente,  
    entonces la variable aleatoria
```
F = (U / d1) / (V / d2)
```
sigue una **distribución F** con `d1` y `d2` grados de libertad.  
Esto permite determinar si la variabilidad de un conjunto de datos es significativamente mayor que la del otro.
<!--ID: 1752531231507-->



**¿Qué representa el valor F en estadística?** #flashcard
El **valor F**, resultado de la prueba F de Snedecor, se calcula como:
```
F = Varianza 1 / Varianza 2
```
donde
- **Varianza 1**: varianza del primer conjunto de datos.
- **Varianza 2**: varianza del segundo conjunto de datos.
- **Valores F altos**: indican que la variabilidad del primer conjunto es mayor que la del segundo, lo que sugiere diferencias significativas.
- **Valores F bajos**: indican que la variabilidad es similar, sin evidencias de diferencias significativas.
<!--ID: 1752531261258-->


---

**¿Cuáles son las características principales de la distribución F?** #flashcard
- **No negativa:** solo toma valores ≥ 0.
- **Asimétrica:** tiene una cola larga hacia la derecha.
- **Dos grados de libertad:** depende de `d1` (numerador) y `d2` (denominador).
- **Valor esperado:**
    ```
    E[F] = d2 / (d2 - 2),   para d2 > 2
    ```
- **Varianza:** fórmula más compleja que depende de `d1` y `d2`.
- Cuando `d2 → ∞`, entonces `d1 * F` se aproxima a una distribución Chi-Cuadrado con `d1` grados de libertad.
<!--ID: 1752531231517-->


---

**¿Cómo se usa la distribución F en el análisis de varianza (ANOVA)?** #flashcard
La distribución F es la base de ANOVA, que compara las medias de dos o más grupos para ver si hay diferencias significativas.
- **Hipótesis nula:** todas las medias son iguales.
- **Estadístico F:**
    ```
    F = Varianza entre grupos / Varianza dentro de grupos
    ```
- Bajo H₀, F sigue una distribución F con:
    - `k - 1` grados de libertad en el numerador, donde `k` es el número de grupos.
    - `N - k` grados de libertad en el denominador, donde `N` es el tamaño total de la muestra.
- Si el **valor p** asociado al F calculado es menor que el nivel de significancia (ej. 0.05), se rechaza H₀, concluyendo que al menos una media difiere.
    
<!--ID: 1752531231526-->


**¿Cuáles son los pasos para realizar un test chi cuadrado de independencia?** #flashcard
1. **Calcula las frecuencias esperadas**
    - Usa la fórmula para cada celda de la tabla de contingencia.  
        ![[Pasted image 20250709192012.png]]  
2. **Calcula el estadístico chi cuadrado (Χ²)**
    - Suma las diferencias al cuadrado entre observados y esperados, dividido por los esperados.
3. **Busca el valor crítico de chi cuadrado**
    - Depende del nivel de significancia (α, normalmente 0.05) y los **grados de libertad**.
4. - **Compara el valor calculado con el valor crítico**
    - Ejemplo:  
        Χ² = 9.79  
        Valor crítico = 5.99
    - Como **9.79 > 5.99**, el estadístico es suficientemente grande.
- **Decide si rechazar la hipótesis nula**
    - Si Χ² es **mayor** que el valor crítico → diferencia estadísticamente significativa (**_p_ < α**), se **rechaza H₀** (las variables están relacionadas).
    - Si Χ² es **menor** que el valor crítico → no significativa (**_p_ > α**), **no se rechaza H₀** (no hay evidencia de relación).
<!--ID: 1752112450043-->


**¿Cuáles son los pasos para realizar un test chi cuadrado de bondad de ajuste ?** #flashcard
1. **Calcula las frecuencias esperadas**
    - A veces este paso es el más difícil. Piensa bien qué proporciones esperas según tu **hipótesis nula**.
    - Normalmente, multiplica la proporción esperada de cada grupo por el total de observaciones.
2. **Calcula el estadístico chi cuadrado (Χ²)**  
    ![[Pasted image 20250709162252.png]]
3. **Busca el valor crítico de chi cuadrado**
    - Depende del nivel de significancia (α, normalmente 0.05) y los **grados de libertad**.
    - Ejemplo con Python para df = 2:
    ```python
    from scipy.stats import chi2
    chi2.ppf(0.95, df=2)  # ≈ 5.99
    ```
4. **Compara el valor calculado con el valor crítico**
    - Ejemplo:  
        Χ² = 1.52  
        Valor crítico = 5.99
    - Como **1.52 < 5.99**, no es lo suficientemente grande.
5. **Decide si rechazar la hipótesis nula**
    - Si Χ² es **mayor** que el valor crítico → diferencia estadísticamente significativa (**_p_ < α**), se **rechaza H₀**.
    -  Si Χ² es **menor** que el valor crítico → no significativa (**_p_ > α**), **no se rechaza H₀**.
<!--ID: 1752112595867-->



**¿Cuáles son las hipótesis en un test chi cuadrado de independencia?** #flashcard
- **Hipótesis nula (H₀):**  
    Las variables **no están relacionadas** en la población; las proporciones de la variable 1 son **iguales para los distintos valores de la variable 2**.
- **Hipótesis alternativa (Hₐ):**  
    Las variables **sí están relacionadas** en la población; las proporciones de la variable 1 **no son iguales para los diferentes valores de la variable 2**.
    
<!--ID: 1752112450062-->


---

**¿Cuáles son las hipótesis en un test chi cuadrado de bondad de ajuste?** #flashcard
- **Hipótesis nula (H₀):**  
    La población **sigue la distribución especificada**.
- **Hipótesis alternativa (Hₐ):**  
    La población **no sigue la distribución especificada**
**Ejemplo:**
- **H₀:** La población de perros elige los tres sabores en **proporciones iguales** (p₁ = p₂ = p₃).
- **Hₐ:** La población de perros **no elige** los tres sabores en proporciones iguales.
<!--ID: 1752112450069-->


---

**¿Qué es la hipótesis nula (H₀)?** #flashcard
La **hipótesis nula (H₀)** es una afirmación que se pone a prueba en un análisis estadístico. Normalmente representa **la ausencia de efecto o relación**, o que las cosas se deben al **azar**.
- Es el punto de partida; se asume verdadera hasta que los datos demuestren lo contrario.
- Ejemplo:
    - En un test de bondad de ajuste: “Los perros eligen los sabores en proporciones iguales.”
    - En un test de independencia: “El reciclaje no depende del tipo de intervención.”
<!--ID: 1752112450074-->


---

**¿Qué es la hipótesis alternativa (Hₐ)?** #flashcard
La **hipótesis alternativa (Hₐ)** es la afirmación que se acepta si los datos muestran evidencia suficiente contra la hipótesis nula. Plantea que **hay un efecto, diferencia o relación**.
- Es lo que tratas de demostrar con tu test estadístico.
- Ejemplo:
    - En un test de bondad de ajuste: “Los perros no eligen los sabores en proporciones iguales.”
    - En un test de independencia: “El reciclaje sí depende del tipo de intervención.”
<!--ID: 1752112450078-->


---

**¿Qué es un test no paramétrico?** #flashcard
Un **test no paramétrico** es una prueba estadística que **no asume una forma específica de distribución** (como la normal) para los datos.
- Es útil cuando **no se cumplen los supuestos** de los tests paramétricos (como normalidad o igualdad de varianzas).
- Sin embargo, las conclusiones suelen ser **menos precisas o potentes** que las de tests paramétricos.
Ejemplo:
- El **test chi cuadrado** es no paramétrico y se usa con variables categóricas.
<!--ID: 1752112450087-->


---

**¿Qué es un error tipo I?** #flashcard
Un **error tipo I** ocurre cuando se **rechaza incorrectamente la hipótesis nula**, es decir, se concluye que hay un efecto o diferencia cuando en realidad **no lo hay**.
- También se llama **falso positivo**.
- Su probabilidad está controlada por el **nivel de significancia (α)**.
Ejemplo
- Si α = 0,05, hay un **5% de probabilidad de cometer un error tipo I**, o dicho de otra forma, de rechazar la hipótesis nula por error.
<!--ID: 1752112450092-->


---

**¿Qué significa grados de libertad en chi cuadrado? (con ejemplos)** #flashcard
Los **grados de libertad (df)** en un test chi cuadrado representan la **cantidad de valores independientes** que quedan después de aplicar restricciones.
- En un **test de bondad de ajuste** con _k_ categorías:  
    **df = k - 1**
- En un **test de independencia** con una tabla de r filas y c columnas:  
    **df = (r - 1) × (c - 1)*
**Ejemplos:**
- Si comparas tres sabores de comida para perros (bondad de ajuste):  
    **df = 3 - 1 = 2**
- Si usas una tabla de 3 intervenciones × 2 resultados (sí o no reciclan):  
    **df = (3 - 1) × (2 - 1) = 2 × 1 = 2**
<!--ID: 1752112450098-->


**¿Qué es la distribución chi cuadrado?** #flashcard
Es una **distribución de probabilidad que se utiliza principalmente para realizar pruebas de hipótesis**, no para describir datos del mundo real.  
Se obtiene al tomar muestras de variables normales estándar independientes, elevarlas al cuadrado y sumarlas.
**Parámetro:**
- **k = grados de libertad**, que indica el número de variables normales independientes elevadas al cuadrado y sumadas.
**Ejemplo gráfico:**
- Si tomas una muestra de una normal estándar (Z), la elevas al cuadrado, obtienes una chi cuadrado con k=1.
- Si tomas dos normales independientes, las elevas al cuadrado y las sumas, obtienes chi cuadrado con k=2.
![[Pasted image 20250709153653.png]]  
![[Pasted image 20250709153730.png]]
<!--ID: 1752112450103-->


---

**¿Qué son los grados de libertad?** #flashcard
Los **grados de libertad (df o v)** son el número de piezas de información independientes utilizadas para calcular una estadística.  
Generalmente se calculan como el tamaño de la muestra menos el número de restricciones aplicadas.
- Los grados de libertad siempre son **menores que el tamaño de la muestra**.
- Normalmente se reportan entre paréntesis junto a la estadística calculada.
<!--ID: 1752112450110-->


---

**¿Qué es el nivel de significancia?** #flashcard
El **nivel de significancia (α)** es el máximo riesgo de cometer un **error tipo I** (rechazar una hipótesis nula verdadera) que estás dispuesto a aceptar.  
Usualmente se fija en **0,05 o 5%**.
**Interpretación:**
- Si el _p_ valor es **menor que α**, los resultados son **estadísticamente significativos** y se rechaza la hipótesis nula.
- Si el _p_ valor es **mayor que α**, no se rechaza la hipótesis nula y los resultados **no son estadísticamente significativos**.
    
<!--ID: 1752112450115-->


---

**¿Cuál es la fórmula del estadístico chi cuadrado?** #flashcard
![[Pasted image 20250709161913.png]]
A mayor diferencia entre las frecuencias observadas (_O_) y esperadas (_E_), mayor será el valor de chi cuadrado.
<!--ID: 1752112450119-->


---

**¿Cuáles son los pasos para calcular chi cuadrado?** #flashcard
1. **Crea una tabla** con frecuencias observadas y esperadas.  
    ![[Pasted image 20250709162007.png]]
2. Calcula **_O - E_**.  
    ![[Pasted image 20250709162023.png]]
3. Calcula **(_O - E_)²**.  
    ![[Pasted image 20250709162042.png]]
4. Calcula **(_O - E_)² / E**.  
    ![[Pasted image 20250709162053.png]]
5. Suma estos valores para obtener **Χ²**.  
    ![[Pasted image 20250709162127.png]]
    
<!--ID: 1752112450466-->


---

**¿Qué es el test chi cuadrado de bondad de ajuste?** #flashcard
Es una **prueba de hipótesis para una sola variable categórica**, que verifica si la distribución de una muestra difiere significativamente de una distribución esperada.
**Condiciones para usarlo:**
1. Hipótesis sobre la distribución de **una sola variable categórica**.  
    (Si es continua, se agrupa en intervalos: binning).
2. Muestra **aleatoria**.
3. Al menos **5 observaciones esperadas por grupo**.
    
<!--ID: 1752112450477-->


---

**Ejemplo del test chi cuadrado de bondad de ajuste** #flashcard
Una empresa de comida para perros prueba tres nuevos sabores con **75 perros**, esperando que cada sabor sea elegido por igual (**25 perros por sabor**).
![[Pasted image 20250709161803.png]]
- Calculan Χ² y lo comparan con el valor crítico con **2 grados de libertad** (3 grupos - 1).
``` Python
from scipy.stats import chi2
chi2.ppf(0.95, df=2)  # ≈ 5.99
```
En este caso, Χ² = 1.52 < 5.99, por lo que no se rechaza la hipótesis nula: los perros eligen los sabores por igual.
<!--ID: 1752112450488-->


**¿Cuándo usar el test chi cuadrado de independencia?** #flashcard
1. Hipótesis sobre la **relación entre dos variables categóricas**.
2. Muestra **aleatoria**.
3. Al menos **5 observaciones esperadas** en cada celda de la tabla.
    
<!--ID: 1752112450495-->


---

**Ejemplo de test chi cuadrado de independencia** #flashcard
Una ciudad prueba si un **folleto**, una **llamada telefónica** o **ninguna intervención** cambian el porcentaje de hogares que reciclan.
- Calculan frecuencias esperadas:  
    ![[Pasted image 20250709190405.png]]  
    ![[Pasted image 20250709190431.png]]
- Calculan Χ² y lo comparan con el valor crítico:
```Python
from scipy.stats import chi2
chi2.ppf(0.95, df=2)  # ≈ 5.99
```
Χ² = 9.79 > 5.99 → se rechaza H₀, hay evidencia de que la intervención influye en el reciclaje.
<!--ID: 1752112534702-->



**¿Qué es la distribución normal ?** #flashcard
Es una **distribución de probabilidad continua, simétrica, con forma de campana**, completamente definida por su **media y desviación estándar**.  
**Características:**
- La **media, mediana y moda son iguales**.
- Es **simétrica** alrededor de la media.
- Su forma característica es de **campana**.
- Solo necesitas conocer la media y la desviación estándar para dibujarla.
- Se utiliza para datos **continuos**.
![[Pasted image 20250709202910.png]]
**Nota:** Un gráfico de cuantiles normales (Q-Q plot) muestra una distribución normal como una línea recta; si los datos se desvían, indica que no son normales.
![[Pasted image 20250709202933.png]]
![[Pasted image 20250709202947.png]]
<!--ID: 1752114594403-->



---

**¿Qué es la distribución exponencial?** #flashcard
Es una **distribución de probabilidad continua que modela el tiempo entre sucesos** en un proceso donde los sucesos ocurren de forma continua e independiente a una **tasa media constante (λ)**.  
Se usa principalmente para analizar **tiempos de espera, tiempos de vida o intervalos entre eventos**.
**Ejemplos de preguntas que responde:**
- ¿Cuál es la probabilidad de esperar entre **X** y **Y** minutos para el siguiente suceso?
- ¿Cuál es la probabilidad de que ocurra el suceso en los primeros **X** minutos?
**Ejemplo **
Imagina un centro de atención donde las llamadas siguen una distribución exponencial con tasa media **λ = 3 llamadas por hora**.
- **¿Probabilidad de esperar entre 10 y 20 minutos a la siguiente llamada?**
    1. Convierte a horas: 10 min = 1/6 h, 20 min = 1/3 h.
    2. Fórmula: P(1/6 < X < 1/3) = ∫[1/6 a 1/3] 3e^(-3x) dx
    3. Evalúa: = -e^(-3x) |[1/6 a 1/3]
    4. Calcula: ≈ [e^(-0.5) - e^(-1)] ≈ 0,2325 o 23,25%.
- **¿Probabilidad de recibir una llamada en los primeros 15 min?**
    1. 15 min = 1/4 h.
    2. Usa la FDA: F(1/4) = 1 - e^(-3*(1/4)) = 1 - e^(-0,75)
    3. Calcula ≈ 0,5276 o 52,76%.
<!--ID: 1752111330010-->


---

**¿Cuál es la función de densidad de probabilidad (PDF) de la distribución exponencial?** #flashcard
La **PDF** nos da la probabilidad de que ocurra un evento en un intervalo exacto.
![[Pasted image 20250709151319.png]]
Donde:
- **x** es la variable aleatoria (usualmente tiempo)
- **λ** es la tasa media (λ > 0)
- **e** ≈ 2,71828 (número de Euler)
    
<!--ID: 1752111330014-->


---

**¿Cuál es la función de distribución acumulativa (FDA) de la distribución exponencial?** #flashcard
La **FDA (o CDF)** nos da la probabilidad de que el evento ocurra antes o hasta un tiempo determinado.
![[Pasted image 20250709151337.png]]
<!--ID: 1752111330021-->


---

---

**¿Qué es la distribución uniforme continua?** #flashcard
Es una **distribución de probabilidad continua donde todos los valores dentro de un intervalo tienen la misma probabilidad de ocurrir**.  
Se debe considerar si los extremos son inclusivos o exclusivos según el problema.
Ejemplo de distribución uniforme continua
El tiempo que una persona espera un autobús está uniformemente distribuido entre 0 y 15 minutos (ambos inclusivos).
- **¿Probabilidad de esperar menos de 12,5 minutos?**
![[Pasted image 20250709152035.png]]  
![[Pasted image 20250709152258.png]]  
![[Pasted image 20250709153106.png]]
<!--ID: 1752111330025-->



---

**¿Cuál es la función de la distribución uniforme continua?** #flashcard
![[Pasted image 20250709151843.png]]
Donde:
- **a** = el menor valor posible
- **b** = el mayor valor posible
<!--ID: 1752111330034-->


---

**¿Cuál es la media y la desviación estándar de la distribución uniforme continua?** #flashcard
![[Pasted image 20250709151906.png]]
<!--ID: 1752111330038-->



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



**¿Qué es la distribución geométrica?** #flashcard
Modelo de probabilidad que describe el **número de intentos necesarios para obtener el primer éxito en una serie de experimentos de Bernoulli independientes**, con la misma probabilidad de éxito.
**Características:**
- **Sin memoria:** la probabilidad del siguiente éxito no depende de los fallos anteriores.
**PMF:**  
P(X=k) = (1-p)^(k-1) * p
**CDF:**  
P(X ≤ x) = 1 - (1-p)^x
**Media y varianza:**
- Media:  
    ![[Pasted image 20250705183207.png]]    
- Varianza:  
    ![[Pasted image 20250705183224.png]]
**Ejemplos:**
- Control de calidad: encontrar el primer producto defectuoso.
- Deportes: primer tiro libre acertado tras varios fallos.
<!--ID: 1751763402507-->




**¿Qué es la distribución hipergeométrica?** #flashcard
Es un **modelo discreto para calcular la probabilidad de obtener un número específico de éxitos en una muestra sin reemplazo de una población finita**.
**Características:**
- **Muestreo sin reemplazo:** la probabilidad cambia en cada extracción.
- Se usa en poblaciones finitas.
- Dos resultados posibles: éxito o fracaso.
**Fórmula:**  
![[Pasted image 20250705183431.png]]
**Media y varianza:**
- Media: μ = n * (k/N)
- Varianza:  
    ![[Pasted image 20250705184431.png]]    
**Ejemplo:**  
De 20 piezas, hay 2 defectuosas. Al inspeccionar 15, calcular la probabilidad de que se rechace el lote.  
![[Pasted image 20250705183707.png]]
**Nota:** Si N > 10n, se puede aproximar por una binomial con p = k/N.
<!--ID: 1751763368599-->



**¿Cual es la formula de nCr?** #flashcard
![[Pasted image 20250705182105.png]]
<!--ID: 1751763368605-->


**¿Qué es la esperanza matemática (valor esperado) y cómo se diferencia de la media?** #flashcard
La **esperanza matemática** es el promedio ponderado de todos los valores posibles que puede tomar una variable aleatoria, según sus probabilidades. Es un concepto teórico.
La **media** es el promedio calculado con datos observados (muestra).
**Ejemplo sencillo:**
- Si un dado tiene números 1 al 6, la esperanza del resultado es el promedio ponderado según sus probabilidades (todas iguales), que es 3.5.
- La media sería, por ejemplo, 3.2 si lanzas el dado 10 veces y haces el promedio de los resultados obtenidos.
<!--ID: 1751763368610-->


¿Qué es la función de densidad de probabilidad? #flashcard
La función de densidad de probabilidad (FDP), en el contexto de la teoría de la probabilidad, ==describe la probabilidad relativa de que una variable aleatoria continua tome un valor específico dentro de un rango dado==. En otras palabras, la FDP es una función que indica la probabilidad de que una variable aleatoria continua se encuentre en un intervalo específico.
Ejemplo:
Si se tiene una FDP que describe la altura de las personas, la FDP mostrará la probabilidad relativa de encontrar a personas con alturas dentro de ciertos rangos. Por ejemplo, podría indicar que es más probable encontrar personas con alturas entre 1.60 y 1.70 metros que entre 1.90 y 2.00 metros
![[función-de-probabilidad-variable-aleatoria-continua-28 1.jpg]]
<!--ID: 1751755620720-->



¿Qué es la función de masa de probabilidad? #flashcard
La función de masa de probabilidad (FMP), también conocida como función de probabilidad o función de cuantía, ==es una función que describe la probabilidad de que una variable aleatoria discreta tome un valor específico==. Para una variable aleatoria discreta X, la FMP, denotada como f(x) o P(X=x), asigna una probabilidad a cada valor posible de x
![[mpf.png]]
<!--ID: 1751755546564-->



**¿Qué es una variable aleatoria?** #flashcard
Es una **función que asigna un valor numérico a cada posible resultado de un experimento aleatorio**.  
Es una forma de cuantificar los resultados de un evento incierto, donde el valor que toma la variable no se conoce con certeza antes de que ocurra el experimento.
Ejemplo:
- Al lanzar un dado, la variable aleatoria podría ser el número que aparece en la cara superior, que puede ser 1, 2, 3, 4, 5 o 6.
    
<!--ID: 1751755201301-->


**¿Qué es una variable aleatoria discreta?** #flashcard
Es una variable aleatoria que **solo puede tomar un número finito o infinito numerable de valores**, generalmente números enteros.  
Cada valor representa un resultado posible de un experimento aleatorio, y se le puede asignar una probabilidad.
Ejemplos:
- El número de caras al lanzar una moneda varias veces.
- El número de clientes que llegan a una tienda en una hora.
- El número de errores en una página de texto.
- El número de hijos en una familia.
    
<!--ID: 1751755152819-->


**¿Qué es una variable aleatoria continua?** #flashcard
Es una variable aleatoria que **puede tomar cualquier valor dentro de un intervalo continuo de números reales**.  
A diferencia de las discretas, tiene infinitos valores posibles entre dos puntos.
Ejemplos:
- **Estatura:** la altura de una persona puede ser 1.60 m, 1.65 m, 1.675 m, etc.
- **Temperatura:** la temperatura de un ambiente puede variar continuamente dentro de un rango.
<!--ID: 1751755152823-->



**¿Por qué son importantes las variables aleatorias en ciencia de datos?** #flashcard
Porque permiten modelar la incertidumbre y describir fenómenos aleatorios cuantitativamente.  
Son la base para construir distribuciones de probabilidad, que a su vez se usan en algoritmos de machine learning, inferencia estadística y simulaciones.
<!--ID: 1751755152826-->



**¿Para qué sirve el teorema de Bayes?** #flashcard
Permite calcular la probabilidad de un evento dado cierto conocimiento previo o evidencia, **actualizando nuestras creencias a medida que obtenemos nueva información**.  
Sirve para calcular lo contrario de la probabilidad condicional directa.
<!--ID: 1751753721840-->

**¿Cuál es la fórmula del teorema de Bayes y qué significa cada término?** #flashcard
P(A|B) = P(B|A) * P(A) / P(B)  
Donde:
- P(A|B) es la probabilidad del evento A dado que el evento B ha ocurrido (probabilidad posterior).
- P(B|A) es la probabilidad del evento B dado que el evento A ha ocurrido (probabilidad condicional).
- P(A) es la probabilidad inicial o probabilidad previa del evento A (antes de considerar la evidencia B).
- P(B) es la probabilidad del evento B (probabilidad de la evidencia total).
Ejemplo:
Supongamos que un laboratorio tiene tres máquinas (A, B y C) que producen envases:
- Máquina A: produce el 40% y tiene un 2% de defectos.
- Máquina B: produce el 30% con un 3% de defectos.
- Máquina C: produce el 30% con un 5% de defectos.
Si se selecciona un envase al azar y está defectuoso, ¿cuál es la probabilidad de que lo haya producido la máquina A?
Datos:  
P(A) = 0.40  
P(D | A) = 0.02  
P(D) = 0.40 x 0.02 + 0.30 x 0.03 + 0.30 x 0.05 = 0.008 + 0.009 + 0.015 = 0.032
Entonces:  
P(A | D) = 0.40 x 0.02 / 0.032 = 0.008 / 0.032 = 0.25 o 25%
    
<!--ID: 1751753721860-->


**¿Cómo saber cuándo utilizar el teorema de Bayes?** #flashcard 
Se usa cuando necesitas determinar la probabilidad de que algo ocurra **dado que existe otra condición que puede influir en dicha ocurrencia**, es decir, para invertir la probabilidad condicional usando la información disponible.
<!--ID: 1751753721864-->



**¿Por qué es importante el teorema de Bayes en ciencia de datos?** #flashcard
Porque permite actualizar probabilidades cuando se obtiene nueva evidencia, y es la base de modelos probabilísticos como el **clasificador Naive Bayes**, que se usa en tareas de clasificación (por ejemplo, filtrado de spam, análisis de sentimientos, diagnóstico médico, etc.).
<!--ID: 1751753721869-->



**¿Qué es una probabilidad previa (prior) y una posterior (posterior) en Bayes?** #flashcard
- La **probabilidad previa** (P(A)) es la creencia inicial sobre A antes de ver la evidencia B.
- La **probabilidad posterior** (P(A|B)) es la creencia actualizada después de incorporar la evidencia B usando el teorema de Bayes.
<!--ID: 1751753721872-->


**¿Qué son eventos mutuamente excluyentes?** #flashcard
Son eventos que **no pueden ocurrir al mismo tiempo**, es decir, no tienen resultados en común.  
Matemáticamente:
P(A∩B)=0 
Un ejemplo clásico es lanzar una moneda: solo puede caer cara o cruz, no ambas a la vez
<!--ID: 1751752589244-->


**¿Qué significa independencia de eventos?** #flashcard
Dos eventos son independientes si la ocurrencia de uno **no afecta la probabilidad** de que ocurra el otro.  
Matemáticamente: P(A∣B)=P(A)
o
P(A∩B)=P(A)×P(B)
<!--ID: 1751752589248-->


**¿Qué es la probabilidad condicional?** #flashcard
Es la probabilidad de que ocurra un evento A dado que ya ha ocurrido otro evento B.  
Se denota como:
<!--ID: 1751752152194-->


**¿Cuál es el teorema de multiplicación para probabilidad condicional?** #flashcard
Indica que:
Permite calcular la probabilidad conjunta a partir de la probabilidad condicional.
<!--ID: 1751752152199-->


**¿Qué dice la regla de la cadena para tres eventos?** #flashcard
Para eventos A, B y C:
<!--ID: 1751752152203-->



¿Qué es un fenómeno aleatorio? #flashcard
Es un experimento o proceso cuyo resultado no se puede predecir con certeza, aunque se repita bajo las mismas condiciones.  
Ejemplo: lanzar un dado, extraer una carta.
<!--ID: 1751749951756-->


¿Qué es el espacio muestral en probabilidad? #flashcard
Es el conjunto de todos los posibles resultados de un fenómeno aleatorio.  
Ejemplo: al lanzar un dado, S={1,2,3,4,5,6}S = \{1,2,3,4,5,6\}S={1,2,3,4,5,6}.
<!--ID: 1751749951773-->


¿Qué es un evento en probabilidad? #flashcard
Es un subconjunto del espacio muestral.  
Un evento ocurre si el resultado del experimento pertenece a dicho subconjunto.  
Ejemplo: el evento "salir número par" al lanzar un dado es A={2,4,6}A = \{2,4,6\}A={2,4,6}.
<!--ID: 1751749951779-->


¿Qué significa calcular la probabilidad de un evento? #flashcard
Es asignar un valor numérico entre 0 y 1 que mide la posibilidad de ocurrencia de un evento.  
En un espacio equiprobable, se calcula como:
​
<!--ID: 1751749951784-->


¿Qué es un gráfico de barras y para qué se usa? #flashcard
Es una representación que muestra cantidades o frecuencias comparando categorías mediante barras rectangulares.  
Se usa para datos categóricos o discretos, ideal para comparar grupos.
<!--ID: 1751675245559-->


¿Qué es un histograma y para qué se usa? #flashcard
Es un gráfico que muestra la distribución de frecuencias de datos numéricos en intervalos continuos.  
Permite analizar la forma de la distribución, detectar asimetrías, curtosis o concentraciones.
<!--ID: 1751675245567-->


¿Qué es un diagrama de caja (box plot) y para qué se usa? #flashcard
Es un gráfico que muestra la mediana, cuartiles, rangos y posibles valores atípicos.  
Se usa para comparar distribuciones y detectar outliers.
<!--ID: 1751675245573-->


¿Qué es un gráfico de líneas y para qué se usa? #flashcard
Representa datos mediante puntos conectados por líneas, mostrando cómo cambian en el tiempo. 
Ideal para series temporales o tendencias.
<!--ID: 1751675245580-->


¿Qué es un gráfico de pastel o tarta y para qué se usa? #flashcard
Muestra proporciones relativas de un total, cada “rebanada” representa una parte del conjunto.  
Se usa para ver la distribución porcentual entre categorías.
<!--ID: 1751675245585-->


¿Qué es un gráfico de dispersión y para qué se usa? #flashcard
Representa puntos en un plano cartesiano según dos variables numéricas.  
Se usa para identificar relaciones, correlaciones o patrones entre variables.
<!--ID: 1751675245591-->


¿Qué es un mapa de calor (heatmap) y para qué se usa? #flashcard
Representa valores con una escala de colores en una matriz o espacio.  
Se usa para ver concentraciones, patrones o intensidad de datos.
<!--ID: 1751675245596-->


¿Qué es una pirámide de población y para qué se usa? #flashcard
Gráfico con forma de pirámide que muestra la distribución de la población por edad y sexo.  
Se usa en análisis demográficos y estudios poblacionales.
<!--ID: 1751675245601-->


¿Qué es un gráfico de Pareto y para qué se usa? #flashcard
Combina barras ordenadas de mayor a menor con una línea acumulada.  
Se usa para aplicar el principio de Pareto (80/20) y priorizar problemas o causas.
<!--ID: 1751675245607-->


¿Qué es una visualización interactiva y para qué se usa? #flashcard
Gráfico dinámico que permite al usuario explorar datos filtrando o destacando información.  
Se usa en dashboards y análisis exploratorios para tomar decisiones.
<!--ID: 1751675245612-->


¿Cuál es la definición del rango en estadística y qué intuición nos da? #flashcard
Es la diferencia entre el valor máximo y el valor mínimo de un conjunto de datos.  
Intuición: muestra el intervalo total que cubren los datos, pero no dice nada sobre cómo están distribuidos dentro de ese rango.
<!--ID: 1751675751966-->


¿Qué es la varianza y cómo podemos entenderla intuitivamente? #flashcard
Es el promedio de las desviaciones al cuadrado respecto a la media.  
Intuición: mide cuánto se dispersan o separan los datos respecto a la media; cuanto mayor sea, más alejados están los valores de su promedio.
<!--ID: 1751675751974-->



¿Qué representa la desviación estándar y cómo se interpreta? #flashcard
Es la raíz cuadrada de la varianza.  
Intuición: indica en promedio cuánto se alejan los datos de la media, expresado en las mismas unidades que los datos originales, lo que facilita su interpretación.
<!--ID: 1751675751978-->



¿Qué indica el coeficiente de variación y cuál es su utilidad? #flashcard
Es la relación entre la desviación estándar y la media, expresada como proporción o porcentaje.  
Intuición: permite comparar la variabilidad entre conjuntos de datos con medias diferentes, mostrando la dispersión relativa.
<!--ID: 1751675751984-->



¿Qué mide el sesgo en estadística y cómo se interpreta su signo? #flashcard
Mide la asimetría de una distribución en relación con su media.  
Intuición: indica si los datos tienen una cola más larga hacia un lado, mostrando hacia dónde se “inclina” la distribución.
- Sesgo positivo: la cola es más larga hacia la derecha, la media > mediana.
- Sesgo negativo: la cola es más larga hacia la izquierda, la media < mediana.  
    El primer coeficiente de asimetría de Pearson se usa si hay una moda clara; si hay varias modas, se recomienda otro enfoque.
    
<!--ID: 1751675751990-->


¿Qué es la curtosis y qué nos permite analizar? #flashcard
Mide el grado de concentración de los datos alrededor de la media y el peso de las colas de la distribución, comparado con la normal.  
Intuición: indica si hay picos muy altos o colas pesadas (más datos extremos) o si la distribución es más plana.
- Mesocúrtica: similar a la normal.
- Leptocúrtica: pico agudo y colas pesadas, más valores extremos.
- Platicúrtica: pico bajo y colas ligeras, menos valores extremos.
    
<!--ID: 1751675751995-->


¿Qué es la media y en qué casos se recomienda usarla? #flashcard
Es la suma de todos los datos dividida entre el número total de datos.  
Ventajas: usa toda la información disponible, fácil de calcular y entender.  
Desventajas: sensible a valores extremos (outliers).  
Uso recomendado: cuando los datos son simétricos y sin valores atípicos.
<!--ID: 1751675752002-->



¿Qué es la mediana y cuándo es más adecuada? #flashcard
Es el valor que ocupa el lugar central cuando los datos están ordenados.  
Ventajas: no se ve afectada por valores extremos.  
Desventajas: no utiliza todos los valores (solo su posición).  
Uso recomendado: cuando hay datos asimétricos o con outliers.
<!--ID: 1751675752013-->


¿Qué es la moda y en qué situaciones se utiliza? #flashcard
Es el valor o valores que más se repiten en el conjunto de datos.  
Ventajas: útil para variables cualitativas o para conocer lo más frecuente.  
Desventajas: puede no existir o haber más de una, no siempre representa bien la distribución.  
Uso recomendado: cuando interesa saber el dato más común o se trabaja con datos categóricos.
<!--ID: 1751675752018-->



¿Qué son las variables cualitativas y cómo se caracterizan? #flashcard
Describen características, cualidades o atributos y no pueden ser medidas con números.  
Pueden ser ordinales o nominales.  
Ej: color de ojos de una persona, raza de un perro.
<!--ID: 1751675752025-->



¿Qué son las variables cuantitativas y qué tipos existen? #flashcard
Se expresan mediante un número, por lo tanto se pueden realizar operaciones con ellas.  
Pueden ser discretas o continuas.  
Ej: el peso de alguien, el número de hijos de una familia, velocidad de un objeto.
<!--ID: 1751675752030-->


¿Qué es una variable cuantitativa discreta y un ejemplo? #flashcard
Es aquella que puede asumir un número contable de valores.  
Ej: número de hijos de una familia, cantidad de dedos en la mano, número de faltas en un partido de fútbol.
<!--ID: 1751675752036-->



¿Qué es una variable cuantitativa continua y un ejemplo? #flashcard
Es aquella que puede asumir un número incontable de valores, incluyendo fracciones o decimales.  
Ej: velocidad a la que va un tren, longitud en centímetros de un tenedor, tiempo que demora un delivery.
<!--ID: 1751675752043-->




