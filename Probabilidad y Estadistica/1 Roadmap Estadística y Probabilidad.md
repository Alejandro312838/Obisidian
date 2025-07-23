# **Hoja de Ruta de Aprendizaje: Probabilidad y Estadística para Ciencia de Datos**

La ciencia de datos es un campo en constante evolución que transforma grandes volúmenes de información en conocimiento accionable. En el corazón de esta disciplina se encuentran la probabilidad y la estadística, dos pilares fundamentales que permiten a los profesionales no solo comprender los datos, sino también extraer valor, identificar patrones y tomar decisiones informadas. Esta hoja de ruta detalla un camino estructurado para dominar estos campos esenciales, destacando su interconexión y su aplicación práctica en el ecosistema de la ciencia de datos.

## **Introducción: La Esencia de la Probabilidad y Estadística en Ciencia de Datos**

La probabilidad y la estadística, aunque estrechamente relacionadas, poseen definiciones y enfoques distintos que se complementan en el análisis de datos. La **probabilidad** se define como la medida de cuán posible es que ocurra un evento determinado cuando el resultado es incierto.1 Es, en esencia, la ciencia de la incertidumbre, que ayuda a cuantificar la posibilidad de que algo suceda.3 Por ejemplo, la probabilidad de obtener "águila" al lanzar una moneda es del 50%.2 Por otro lado, la  
**estadística** es el análisis de eventos gobernados por la probabilidad.1 Su función principal es recolectar, organizar, analizar e interpretar datos numéricos con el objetivo de describir características de una población o sacar conclusiones sobre ella.6 La estadística descriptiva, en particular, se basa en la precisión para describir los datos.7  
La relación entre ambas es simbiótica. Mientras que la probabilidad permite prever qué tipo de datos se observarán si se asume cómo funcionan las cosas, la estadística ayuda a generalizar cómo funcionan las cosas a partir de los datos observados.5 Esta interdependencia es un pilar fundamental para la toma de decisiones basada en datos. La capacidad de cuantificar la incertidumbre a través de la probabilidad habilita decisiones estadísticas robustas, trascendiendo la mera descripción para adentrarse en la predicción y la inferencia. Un profesional de datos debe comprender que estas disciplinas no son temas secuenciales aislados, sino que se entrelazan profundamente para sustentar todo el flujo de trabajo de la ciencia de datos, desde la comprensión inicial de los datos hasta el despliegue de modelos y la formulación de decisiones. Su poder combinado es indispensable para el análisis predictivo y la evaluación de riesgos.  
La importancia de estos campos en el ecosistema de la ciencia de datos es innegable. Son las herramientas necesarias para transformar datos crudos en información útil y tomar decisiones informadas en un mundo saturado de información.6 Permiten identificar patrones (como la correlación), modelar relaciones (mediante regresión), agrupar datos similares (a través del análisis de  
*clusters*), evaluar afirmaciones (con pruebas de hipótesis) y proporcionar rangos de valores para parámetros poblacionales (mediante intervalos de confianza).6 Estas bases teóricas son los cimientos sobre los cuales se construyen diversas metodologías indispensables en la estadística moderna y en la ciencia de datos.9 Un científico de datos, a diferencia de un analista de datos que se enfoca en una única fuente, necesita una visión global y vastos conocimientos en matemáticas, probabilidad y estadística para entender y presentar los datos de la manera más adecuada.10 Estos conocimientos son cruciales para el análisis y la visualización de cualquier colección de datos, permitiendo descubrir resultados que generen valor o revelen narrativas significativas.4 La probabilidad, en particular, es esencial para aplicar conceptos como la estadística inferencial y las redes bayesianas, que son cruciales para las predicciones.4  
El rol del científico de datos ha evolucionado significativamente, y con ello, la necesidad de una comprensión conceptual profunda. El valor de un científico de datos radica en su capacidad para comprender los principios matemáticos y estadísticos subyacentes, lo que le permite interpretar resultados, optimizar modelos y comunicar hallazgos de manera efectiva a audiencias no técnicas.11 Esta comprensión es vital para adaptarse a nuevos problemas y fomentar la innovación, en lugar de simplemente aplicar soluciones preexistentes. Por lo tanto, esta hoja de ruta enfatiza el "porqué" detrás de cada concepto, no solo el "qué".

## **Fundamentos Matemáticos Esenciales para la Ciencia de Datos**

**Archivo de Referencia:** [[01_Fundamentos_Matematicos]]

Antes de sumergirse en la probabilidad y la estadística aplicada, es crucial establecer una base sólida en ciertas áreas matemáticas. Si bien no se espera que un científico de datos sea un matemático puro, una comprensión conceptual de estos pilares es indispensable para entender el funcionamiento interno de los algoritmos de Machine Learning y Deep Learning, optimizar modelos y comunicar resultados de manera efectiva.4

### **Álgebra Lineal**

El Álgebra Lineal es un campo de las matemáticas que desempeña un papel fundamental en la inteligencia artificial.12 Es la base de un gran número de conceptos y técnicas en la ciencia de datos.13 Muchos algoritmos de aprendizaje automático requieren una comprensión profunda de sus notaciones y aritmética.12 Los datos numéricos a menudo se representan como vectores o matrices (por ejemplo, \[altura, peso, edad\] como un vector tridimensional), y las operaciones de álgebra lineal son fundamentales para manipular estos datos.13  
Los conceptos clave incluyen:

* **Vectores:** Y sus operaciones como suma, multiplicación, producto escalar y producto vectorial.14 Los vectores son objetos que pueden sumarse y multiplicarse por escalares para formar nuevos vectores, y concretamente, son puntos en un espacio de dimensiones finitas.13  
* **Matrices:** Y sus operaciones como sumas, multiplicación por escalar, producto matricial y matriz inversa.14  
* **Matrices especiales:** Incluyendo identidad, traspuesta, cuadrada, diagonal, fila, columna, triangular superior e inferior.14

El Álgebra Lineal permite entender cómo funcionan los algoritmos de inteligencia artificial internamente, lo que a su vez ayuda a preparar los datos y seleccionar los algoritmos más adecuados.4 Esta área de las matemáticas es la maquinaria subyacente que permite que los algoritmos estadísticos y de aprendizaje automático operen de manera eficiente y efectiva. Sin una comprensión de estos fundamentos, un científico de datos podría usar herramientas, pero le sería difícil optimizar, interpretar o innovar con ellas. Por lo tanto, la hoja de ruta subraya que estos fundamentos matemáticos no son opcionales, sino habilitadores críticos para una comprensión más profunda y una aplicación avanzada en la ciencia de datos. Se prioriza la comprensión conceptual sobre la memorización de fórmulas.11

#### **Matrices de Covarianza**

En estadística y teoría de la probabilidad, la matriz de covarianza es una matriz cuadrada que contiene la covarianza entre los elementos de un vector. Es la generalización natural a dimensiones superiores del concepto de varianza de una variable aleatoria escalar.24 Proporciona una visión integral de las relaciones entre variables.25 Una matriz de covarianza es simétrica y semidefinida positiva.24  
Su aplicación es fundamental en el Análisis de Componentes Principales (PCA), una técnica de reducción de dimensionalidad que busca transformar ortogonalmente los datos para maximizar su varianza.24

#### **Autovalores y Autovectores**

Los autovalores y autovectores son conceptos cruciales en álgebra lineal con amplias aplicaciones en *machine learning*, especialmente en la reducción de dimensionalidad. En el contexto del PCA, los autovectores de una matriz de dispersión (o covarianza) indican las direcciones principales en las que los puntos de datos tienden a alinearse, mientras que los autovalores asociados representan la magnitud de la varianza en esas direcciones.26 El autovector con el mayor autovalor señala la dirección de máxima variabilidad en los datos.26 Estos conceptos permiten reducir la dimensionalidad de vectores grandes manteniendo una cantidad significativa de información.26

#### **Descomposición de Valores Singulares (SVD)**

La Descomposición de Valores Singulares (SVD) es una técnica poderosa en álgebra lineal utilizada para la reducción de dimensionalidad, compresión de datos y reducción de ruido.29 La SVD revela factores inherentes a cualquier conjunto de datos estructurado matricialmente y es fundamental para comprender cómo decaen los valores singulares, lo que tiene profundas repercusiones teóricas.30 También es útil para completar bases de datos con elementos faltantes, proporcionando la mejor predicción posible para esas entradas.30

### **Cálculo**

El Cálculo es otra área matemática vital para la ciencia de datos, especialmente en el contexto de la optimización y el aprendizaje automático.  
Los conceptos clave del Cálculo incluyen:

* **Funciones:** Que describen relaciones entre entradas y salidas.14  
* **Razón de cambio (derivadas):** Permiten entender cómo una variable cambia en relación con otra, lo que se traduce en comprender tendencias y hacer predicciones. Las derivadas parciales y funciones multivariadas son extensiones para manejar múltiples variables independientes.14  
* **Mínimos y máximos locales:** Una aplicación específica de la segunda derivada, vital para la optimización de modelos en ciencia de datos. Por ejemplo, en el aprendizaje automático, se busca minimizar una "función de pérdida" o "función de costo" para mejorar la precisión del modelo.14  
* **Áreas bajo la curva (integrales):** Fundamentales para comprender e interpretar las distribuciones y densidades de probabilidad, y útiles para evaluar el rendimiento de los modelos, como en la curva ROC.14

El Cálculo se utiliza en algoritmos de regresión de machine learning para la predicción de datos y para encontrar el error mínimo, buscando que las predicciones sean lo más precisas posible.4 Esto es particularmente necesario al implementar Deep Learning con redes neuronales.4 La optimización, que busca minimizar o maximizar funciones, está presente en todo momento, con técnicas como el Gradiente Descendente (  
*Gradient Descent*) para encontrar el valor mínimo de funciones de pérdida o costo y mejorar modelos iterativamente.14 La optimización no es simplemente un tema avanzado, sino un proceso central en la mejora iterativa y el refinamiento de los modelos de ciencia de datos. Comprender sus fundamentos matemáticos (cálculo) permite a los científicos de datos ir más allá del uso de modelos de "caja negra" para realizar un ajuste inteligente de hiperparámetros, depuración de modelos y desarrollo de soluciones más robustas y precisas.

### **Otras Áreas Matemáticas Relevantes**

Además del Álgebra Lineal y el Cálculo, otras áreas matemáticas contribuyen significativamente a las habilidades de un científico de datos:

* **Optimización:** Fundamental para el "fine-tuning" de modelos, maximizando métricas relevantes.14  
* **Optimización Convexa:** La Optimización Convexa es un área de las matemáticas aplicadas que se enfoca en minimizar funciones convexas sobre conjuntos convexos. Es de gran interés en ciencia de datos y aprendizaje automático debido a su eficiencia y la garantía de encontrar un óptimo global.31 Sus aplicaciones incluyen la optimización de carteras en finanzas (maximizando retornos y minimizando riesgos) y el diseño de algoritmos eficientes en sistemas de control y procesamiento de señales.32 Algoritmos como el descenso de gradiente, el método de Newton y los métodos de punto interior son comúnmente utilizados para resolver problemas de optimización convexa.32  
* **Diseño Experimental:** Proporciona estrategias para maximizar la calidad y cantidad de información obtenida de experimentos, minimizando costos y estableciendo relaciones causales.14  
* **Muestreo:** Crucial para minimizar el sesgo en los resultados y asegurar la representatividad de la muestra, especialmente en el contexto de Big Data.14  
* **Teoría de Grafos:** Útil para desentrañar patrones en datos con relaciones, aplicable en sistemas de recomendación, detección de anomalías, logística y procesamiento de lenguaje natural.14

## **Módulo 1: Estadística Descriptiva**

**Archivo de Referencia:** [[02_Estadistica_Descriptiva]]

La estadística descriptiva representa el primer paso y el "primer contacto" crítico en el análisis de datos. Su objetivo principal es organizar, resumir y presentar los datos de manera que sus características principales sean fácilmente comprensibles.7 Se considera la estadística "tradicional" y se basa en la precisión para describir los datos.7 Una fase descriptiva exhaustiva es crucial antes de avanzar a modelados más complejos, ya que ayuda a identificar problemas de calidad de datos, comprender distribuciones, detectar valores atípicos y formular hipótesis iniciales. Esta etapa influye directamente en el éxito de las tareas inferenciales y predictivas posteriores.

### **Conceptos Básicos**

* **Población y Muestra:** La estadística descriptiva se enfoca en describir las características de un conjunto de datos, ya sea una población completa o una muestra.6 En contraste, la estadística inferencial busca sacar conclusiones sobre una población más grande a partir del estudio de una muestra.5  
* **Variables y Tipos de Datos:** Es fundamental identificar y diferenciar entre variables cualitativas y cuantitativas, así como entre variables discretas y continuas.15

### **Medidas de Tendencia Central**

Estas medidas permiten identificar el valor más representativo de un conjunto de datos.6

* **Media:** El promedio aritmético, calculado como la suma de los valores dividida por el número total de ellos.7  
* **Mediana:** El valor central de un conjunto de datos ordenado.  
* **Moda:** El valor que aparece con mayor frecuencia en un conjunto de datos.

### **Medidas de Dispersión**

Estas medidas muestran cuán dispersos están los datos alrededor de la media.6

* **Rango:** La diferencia entre el valor máximo y mínimo.  
* **Varianza y Desviación Estándar:** Indican la variabilidad o dispersión de los datos con respecto a la media.6  
* **Sesgo (*Skewness*) y Curtosis (*Kurtosis*):** El sesgo describe la asimetría de la distribución de los datos, mientras que la curtosis se refiere a la "puntiagudez" o "aplanamiento" de la curva de datos, relacionada con la distancia y proximidad de los datos respecto al promedio.7

### **Técnicas de Visualización de Datos para la Exploración Inicial**

Las visualizaciones son esenciales para representar los datos de forma visual y facilitar su comprensión.6

* **Gráficos de Barras, Histogramas y Diagramas de Caja (*Box Plots*):** Los histogramas muestran la frecuencia de valores en un conjunto de datos 5, mientras que los diagramas de caja son útiles para identificar valores atípicos y comparar conjuntos de datos.5  
* **Tipos de Gráficos Avanzados:** Además de los gráficos de barras, histogramas y diagramas de caja, otras visualizaciones importantes incluyen: **gráficos de líneas** (ideales para mostrar tendencias a lo largo del tiempo o secuencia, como series temporales 33),  
  **gráficos de pastel o tarta** (para comparar proporciones entre diferentes categorías, aunque se recomienda precaución con muchas categorías 33),  
  **gráficos de dispersión** (para visualizar la relación entre dos variables numéricas 33),  
  **mapas de calor** (efectivos para visualizar la relación entre dos variables categóricas usando colores para representar frecuencia o densidad 33),  
  **pirámides de población** (histogramas bidireccionales para estructura demográfica por sexo y edad 34), y  
  **gráficos de Pareto** (gráficos de barras verticales ordenados por frecuencias descendentes para identificar y priorizar datos 34).

La visualización interactiva es un catalizador para la comprensión de datos dinámicos. Más allá de los gráficos estáticos, las visualizaciones interactivas son cada vez más vitales en la ciencia de datos. Permiten una exploración más profunda y dinámica, especialmente con conjuntos de datos grandes o en *streaming*. Esta capacidad permite a los científicos de datos identificar patrones y anomalías que podrían pasarse por alto en representaciones estáticas, fomentando una comprensión más intuitiva de comportamientos de datos complejos.

## **Módulo 2: Probabilidad**

**Archivo de Referencia:** [[03_Probabilidad]]

La probabilidad es el lenguaje de la incertidumbre, y su comprensión es fundamental para modelar fenómenos aleatorios, evaluar riesgos y establecer las bases para la estadística inferencial y el aprendizaje automático.1

### **Conceptos Fundamentales**

* **El Fenómeno Aleatorio:** Se refiere a eventos cuyo resultado no puede predecirse con certeza.17  
* **Espacio Muestral y Evento:** El espacio muestral es el conjunto de todos los posibles resultados de un experimento aleatorio. Un evento es un subconjunto de este espacio.17  
* **Axiomas de Probabilidad:** Son las reglas fundamentales que rigen el cálculo de probabilidades.17  
* **Probabilidad de un Evento:** Se calcula como el número de maneras en que un evento puede suceder dividido por el número total de resultados posibles. La probabilidad de un evento siempre es un número entre 0 y 1\.2

### **Probabilidad Condicional e Independencia de Eventos**

* **Probabilidad Condicional:** Permite calcular la probabilidad de que un suceso ocurra dado que otro suceso ya ha ocurrido.17  
* **Eventos Mutuamente Excluyentes e Independencia:** Los eventos mutuamente excluyentes no pueden ocurrir al mismo tiempo. La independencia se refiere a si la ocurrencia de un evento afecta o no la probabilidad de otro.9

### **Variables Aleatorias y las Principales Distribuciones de Probabilidad**

Una **variable aleatoria** es una función definida sobre el espacio muestral que asigna números reales a los resultados de un experimento aleatorio.18 Una  
**distribución de probabilidad** es una descripción matemática de las probabilidades de ocurrencia de posibles resultados en un experimento aleatorio o proceso estocástico.15 Asigna probabilidades o densidades de probabilidad a cada posible resultado de un evento aleatorio.15  
La probabilidad tiene una dualidad crucial: es tanto la cuantificación de la incertidumbre como el fundamento para la inferencia. No solo se trata de calcular las posibilidades, sino de construir modelos de la realidad bajo incertidumbre. Esta comprensión es vital para interpretar intervalos de confianza, valores p y las salidas de modelos predictivos, ya que la probabilidad forma el puente hacia la estadística inferencial.  
Las distribuciones de probabilidad son como las "huellas dactilares" de los datos. Reconocer y comprender las diferentes distribuciones es clave para entender el proceso generativo subyacente de los datos. Esto ayuda a seleccionar las pruebas estadísticas correctas, construir modelos predictivos más precisos y comprender la variabilidad y los patrones inherentes a los datos.

#### **Tipos de Distribuciones:**

* **Discretas:** La función de probabilidad solo toma valores positivos en un conjunto de valores finito o infinito numerable.18 Un ejemplo es la Distribución Binomial.18  
* **Continuas:** La variable puede tomar cualquiera de los infinitos valores existentes dentro de un intervalo.15 La probabilidad de que una variable aleatoria continua tome un valor específico es generalmente cero; se utiliza la función de densidad de probabilidad para calcular la probabilidad de que la variable se encuentre dentro de un intervalo particular mediante integración.15 Ejemplos comunes incluyen la Distribución Normal (también conocida como Gaussiana o la "campana de Gauss"), la Distribución Exponencial, la Uniforme y la Chi-cuadrado.15

#### **Funciones de Probabilidad y Densidad:**

* **Función de Masa de Probabilidad (FMP):** Para variables discretas, indica la probabilidad de que ocurra cada resultado.15  
* **Función de Densidad de Probabilidad (FDP):** Para variables continuas, se utiliza para calcular la probabilidad de que la variable esté dentro de un intervalo particular.15

La siguiente tabla resume algunos tipos comunes de distribuciones de probabilidad y su relevancia en la ciencia de datos:  
**Tabla 2: Tipos de Distribuciones de Probabilidad Comunes y su Relevancia en Ciencia de Datos**

| Distribución | Tipo de Variable | Descripción Clave | Relevancia/Aplicación en Ciencia de Datos |
| :---- | :---- | :---- | :---- |
| **Normal (Gaussiana)** | Continua | Simétrica, en forma de campana, caracterizada por su media y desviación estándar. | Modelado de errores, fenómenos naturales, base para muchas pruebas estadísticas inferenciales, distribución de variables en grandes conjuntos de datos.15 |
| **Binomial** | Discreta | Probabilidad de un número de éxitos en una secuencia fija de ensayos de Bernoulli independientes. | Modelado de resultados binarios (éxito/fracaso), control de calidad, pruebas A/B.18 |
| **Poisson** | Discreta | Probabilidad de un número de eventos que ocurren en un intervalo fijo de tiempo o espacio. | Modelado de eventos raros (ej., llamadas a un *call center*, llegadas de clientes), análisis de incidentes. |
| **Exponencial** | Continua | Describe el tiempo entre eventos en un proceso de Poisson (eventos que ocurren a una tasa constante e independiente). | Modelado de tiempos de vida, tiempos de espera en colas, fiabilidad de componentes.15 |
| **Uniforme** | Continua/Discreta | Todos los resultados posibles tienen la misma probabilidad de ocurrir dentro de un intervalo dado. | Generación de números aleatorios, base para simulación, modelado de incertidumbre sin información previa. |
| **Chi-cuadrado (χ2)** | Continua | Suma de cuadrados de variables aleatorias normales estándar independientes. | Pruebas de bondad de ajuste, pruebas de independencia en tablas de contingencia, intervalos de confianza para varianza.15 |
| **t de Student** | Continua | Similar a la normal, pero con colas más pesadas, utilizada para muestras pequeñas. | Pruebas de hipótesis con muestras pequeñas, intervalos de confianza cuando la desviación estándar poblacional es desconocida. |
| **F** | Continua | Razón de dos variables aleatorias Chi-cuadrado divididas por sus grados de libertad. | Análisis de Varianza (ANOVA) para comparar medias de tres o más grupos, pruebas de significancia en regresión.18 |

#### **Teorema de Bayes**

El **Teorema de Bayes** es una proposición matemática crucial en estadística y cálculo de probabilidad que permite actualizar probabilidades basándose en nueva información.35 Este enfoque es esencial para modelar la incertidumbre y tomar decisiones fundamentadas en datos.35 En  
*machine learning*, el teorema se utiliza en algoritmos como los clasificadores Bayesianos, fundamentales para tareas de clasificación como el filtrado de correo no deseado, el diagnóstico médico de enfermedades y el análisis del comportamiento del cliente.35 Su capacidad para combinar datos previos con evidencia nueva lo hace ideal para análisis predictivos y diagnósticos.35

## **Módulo 3: Estadística Inferencial**

**Archivo de Referencia:** [[04_Estadistica_Inferencial]]

La estadística inferencial es el componente que permite a los científicos de datos trascender la mera descripción y sacar conclusiones sobre una población más grande basándose en el análisis de una muestra más pequeña de datos.5 Esta capacidad es crucial para la toma de decisiones basada en evidencia y para el desarrollo de modelos predictivos.6  
La inferencia es el puente entre los datos y las decisiones estratégicas. Esta rama de la estadística es el vínculo crítico que transforma los hallazgos de datos brutos en estrategias empresariales accionables y afirmaciones validadas. No se trata solo de entender los datos, sino de confiar en los conocimientos derivados de ellos y actuar en consecuencia. Un dominio sólido de la estadística inferencial es crucial para que un científico de datos proporcione recomendaciones fiables y basadas en datos que puedan resistir el escrutinio. Esto incluye comprender las limitaciones de las muestras, los matices de los valores p y la interpretación práctica de los intervalos de confianza en escenarios del mundo real. Se trata de construir modelos que generalicen bien y tomar decisiones con incertidumbre cuantificada.

### **Muestreo y Estimación de Parámetros**

* **Muestreo:** Es la base para sacar conclusiones generales sobre toda la población a partir del estudio de una muestra.5 Es crucial para minimizar el sesgo y asegurar la representatividad de la muestra.14  
* **Estimación de Parámetros:** Permite estimar características desconocidas de una población a partir de datos de una muestra.5 Métodos como la máxima verosimilitud son herramientas comunes para esto.20

El muestreo y el diseño experimental actúan como guardianes de la calidad y validez de la inferencia. Un error común en la ciencia de datos es extraer conclusiones incorrectas de datos sesgados o mal recolectados. Un profundo conocimiento de las técnicas de muestreo y del diseño experimental no es un ejercicio teórico, sino una necesidad práctica para garantizar la validez y fiabilidad de las inferencias estadísticas. Este enfoque proactivo en la recolección y preparación de datos impacta directamente en la confiabilidad y aplicabilidad de cualquier conocimiento o modelo derivado.

### **Pruebas de Hipótesis**

* **Conceptos:** Las pruebas de hipótesis permiten evaluar si una afirmación sobre una población es verdadera o falsa.5 Consisten en validar conclusiones construidas a partir de una porción de datos.7  
* **Tipos y Aplicación:** Incluyen pruebas paramétricas y no paramétricas.20 Es esencial comprender los diferentes tipos de pruebas de hipótesis, el concepto de valor p y los intervalos de confianza asociados.11 Son cruciales para la experimentación de producto y el diseño y aplicación de experimentos.11  
* **Errores en Pruebas de Hipótesis:** Al realizar pruebas de hipótesis, es fundamental comprender los tipos de errores que se pueden cometer:  
  * **Error de Tipo I (α):** Se produce cuando se rechaza incorrectamente una hipótesis nula verdadera (falso positivo).37 La probabilidad de cometer este error se establece comúnmente en 0.05.37  
  * **Error de Tipo II (β):** Ocurre cuando no se rechaza una hipótesis nula falsa (falso negativo).37 La probabilidad de este error depende de la magnitud del efecto de interés y del tamaño de la muestra.38

### **Intervalos de Confianza**

Los intervalos de confianza proporcionan un rango de valores dentro del cual se espera que se encuentre un parámetro poblacional con un cierto nivel de confianza.6 Son una herramienta clave para cuantificar la incertidumbre de una estimación.

### **Análisis de Regresión y Correlación**

* **Correlación:** Mide la fuerza y dirección de la relación lineal entre dos variables.6 La covarianza, por ejemplo, indica el sentido de la correlación.5  
* **Regresión:** Permite modelar la relación entre una variable dependiente y una o más variables independientes.6 La regresión lineal es una de las técnicas más simples y ampliamente utilizadas.5

## **Módulo 4: Aplicaciones Avanzadas en Ciencia de Datos**

**Archivo de Referencia:** [[05_Aplicaciones_Avanzadas]]

Con una base sólida en probabilidad y estadística, el estudiante estará preparado para explorar cómo estos conceptos se aplican en áreas más avanzadas de la ciencia de datos, como el aprendizaje automático y el análisis de datos complejos.

### **Estadística para Machine Learning y Deep Learning**

La estadística inferencial es el punto donde los modelos de probabilidades y las técnicas de *machine learning* e inteligencia artificial, así como los modelos predictivos, cobran vida.7 El Álgebra Lineal es necesaria para comprender la estadística, un campo importante en el aprendizaje automático.12 Los algoritmos matemáticos para el desarrollo de modelos predictivos y la automatización requieren conocimientos estadísticos profundos.10  
La estadística es el "lenguaje interno" de los algoritmos de Machine Learning y Deep Learning. Estos algoritmos no son "cajas negras" incomprensibles; en su núcleo, son modelos estadísticos. Comprender los principios estadísticos (como distribuciones, regresión, pruebas de hipótesis) permite a un científico de datos entender por qué ciertos algoritmos se comportan de una manera determinada, cómo interpretar sus resultados y cuándo aplicarlos de manera apropiada. Para una aplicación efectiva e innovadora en ML/DL, un científico de datos debe ir más allá del mero uso de librerías y alcanzar una comprensión conceptual de los mecanismos estadísticos subyacentes. Esto permite una selección informada de modelos, un ajuste preciso de hiperparámetros, la detección de sesgos y una interpretación robusta de los resultados, lo cual es crucial para construir sistemas de IA confiables.

### **Regresión Logística**

A diferencia de la regresión lineal, que predice valores continuos, la **regresión logística** es un algoritmo de clasificación que modela la probabilidad de que una variable dependiente binaria (o categórica) ocurra.39 No puede predecir los valores reales de datos continuos, sino que responde a preguntas con resultados discretos (ej., sí/no, fraudulento/no fraudulento).39  
Sus aplicaciones son diversas, incluyendo la estimación de la probabilidad de fallo de piezas en fabricación, la predicción de enfermedades en sanidad, el análisis de transacciones financieras para detectar fraudes, y la predicción de clics en anuncios en marketing.39  
Para su aplicación, es importante considerar ciertas condiciones: **no colinealidad o multicolinealidad** entre predictores (para evitar que la información de una variable sea redundante y afecte la significancia de los coeficientes), **relación lineal** entre los predictores numéricos y el logaritmo de *odds* de la variable respuesta, **no autocorrelación** (independencia de las observaciones, crucial en series temporales), la identificación de **valores atípicos** o influyentes, y un **tamaño de muestra** adecuado (se recomienda que el número de observaciones sea al menos 10 a 20 veces el número de predictores).40 La  
**parsimonia** también es clave, buscando el modelo más simple que explique la variabilidad observada.40

### **Métricas de Evaluación de Modelos**

La evaluación de modelos es una etapa crítica en la ciencia de datos para cuantificar el rendimiento y la fiabilidad de los modelos predictivos. Las métricas varían según el tipo de problema (regresión o clasificación).

#### **Para Modelos de Regresión:**

* **Error Cuadrático Medio (MSE \- Mean Squared Error):** Mide la magnitud de los errores al promediar el cuadrado de las diferencias entre valores reales y predicciones. Un MSE bajo indica predicciones cercanas a los valores reales.41  
* **Error Absoluto Medio (MAE \- Mean Absolute Error):** Mide la diferencia promedio absoluta entre valores reales y predichos. Es más robusto frente a valores atípicos que el MSE, ya que no eleva los errores al cuadrado.41  
* **Raíz del Error Cuadrático Medio (RMSE \- Root Mean Square Error):** Es la raíz cuadrada del MSE, lo que permite que la métrica esté en las mismas unidades que la variable objetivo, facilitando la interpretación.41  
* **Coeficiente de Determinación (R² \- R-Squared):** Indica la proporción de la varianza en la variable dependiente que es predecible a partir de las variables independientes. Un R² de 1 significa que el modelo explica el 100% de la variabilidad, mientras que 0 indica que no explica ninguna.41  
* **Coeficiente de Correlación de Pearson:** Mide la fuerza y dirección de la relación lineal entre las predicciones y los valores reales. Un valor cercano a 1 o \-1 indica una fuerte correlación lineal.41

#### **Para Modelos de Clasificación:**

* **Matriz de Confusión:** Una tabla que resume el rendimiento de un algoritmo de clasificación, mostrando los verdaderos positivos (TP), verdaderos negativos (TN), falsos positivos (FP) y falsos negativos (FN).43  
* **Precisión (Accuracy):** El porcentaje total de elementos clasificados correctamente. Es una medida directa de la calidad, pero puede ser engañosa en conjuntos de datos desequilibrados.43  
* **Sensibilidad (Recall o TPR \- True Positive Rate):** El número de elementos identificados correctamente como positivos del total de positivos verdaderos.43  
* **Especificidad (TNR \- True Negative Rate):** El número de elementos identificados correctamente como negativos del total de negativos verdaderos.43  
* **Precisión (Precision):** El número de elementos identificados correctamente como positivos de un total de elementos identificados como positivos.43  
* **F1-Score:** Una media armónica de la precisión y la sensibilidad, útil para equilibrar ambas métricas, especialmente en problemas con clases desequilibradas.43  
* **Área bajo la Curva ROC (AUC-ROC \- Area Under the Receiver Operating Characteristic Curve):** Mide la capacidad de un clasificador para distinguir entre clases, representando la relación entre la tasa de verdaderos positivos y la tasa de falsos positivos en diferentes umbrales.43

### **Diseño Experimental y Pruebas A/B**

El diseño experimental es crucial para establecer relaciones causales entre variables de manera efectiva, maximizando la calidad de la información obtenida.14 Las pruebas de hipótesis son esenciales para la experimentación de producto y el diseño y aplicación de experimentos, permitiendo a los científicos de datos en experimentación de producto enfocarse en el testeo de hipótesis.11  
La transición de la predicción a la prescripción se logra a través del diseño experimental. Mientras que los modelos predictivos nos dicen "qué podría suceder", los modelos prescriptivos (a menudo informados por el diseño experimental) nos indican "qué deberíamos hacer". La capacidad de establecer causalidad mediante experimentos bien diseñados es una habilidad de orden superior que va más allá de la mera correlación o predicción. Esto eleva el rol del científico de datos de un simple analista a un asesor estratégico, capaz de diseñar intervenciones y medir su impacto causal, lo cual es altamente valorado en entornos empresariales.

### **Análisis de Series Temporales**

El análisis de series temporales es fundamental para comprender y modelar datos que evolucionan con el tiempo. Esto incluye técnicas para la generación de intervalos de fechas, conversión de frecuencias, estadísticas de ventanas móviles, y el desplazamiento de fechas y desfase. Modelos como ARIMA (media móvil integrada autorregresiva) y métodos de suavizado exponencial son comúnmente utilizados para la predicción y el análisis de tendencias en datos temporales.

### **Análisis de *Clusters***

Esta técnica agrupa datos similares en categorías.6 Dentro del análisis de  
*clusters*, el algoritmo **K-medias (K-means)** es uno de los métodos de agrupación no supervisada más populares.44 Su objetivo es encontrar agrupamientos o patrones subyacentes en datos no etiquetados, dividiendo un conjunto de datos en  
*k* grupos similares basados en la distancia a sus centroides.44  
El algoritmo funciona de manera iterativa: primero se inicializan *k* centroides (puntos centrales de los *clusters*), luego cada punto de datos se asigna a su centroide más cercano, y finalmente los centroides se recalculan como la media de todos los puntos asignados a ese *cluster*.44 Este proceso se repite hasta que las posiciones de los centroides convergen.44  
La elección del número *k* de *clusters* es una suposición clave del algoritmo.45 Para evaluar la calidad de la agrupación, se utilizan métricas como la  
**inercia**, que mide cuán compactos son los puntos de datos dentro de un *cluster* (distancia intracluster, se busca minimizarla) 44, y el  
**índice de Dunn**, que representa la relación entre la distancia mínima entre *clusters* y la distancia máxima dentro de *clusters* (se busca maximizarlo para indicar *clusters* bien separados).44 La inicialización de los centroides puede influir en los resultados, y métodos como  
*k-means++* buscan mitigar la aleatoriedad.44

## **Consejos para un Aprendizaje Efectivo y Continuo**

**Archivo de Referencia:** [[06_Consejos_Aprendizaje]]

Para dominar la probabilidad y la estadística en el contexto de la ciencia de datos, es crucial adoptar un enfoque de aprendizaje estratégico y continuo.

### **Enfoque en la Comprensión Conceptual sobre la Memorización de Fórmulas**

Es fundamental entender el concepto general, analizar la fórmula, comprender los símbolos matemáticos y la lógica subyacente de su funcionamiento, en lugar de dedicar tiempo a la memorización.11 La comprensión de los principios del cálculo, por ejemplo, es crucial para entender cómo afectan los modelos y cómo utilizarlos para interpretar resultados de manera más precisa.14 La "mentalidad de científico de datos" trasciende el mero conocimiento técnico. La habilidad para abstraer, interpretar y comunicar hallazgos complejos a una audiencia no técnica es tan crítica como la pericia técnica. Este enfoque holístico asegura que el conocimiento estadístico adquirido pueda ser efectivamente aprovechado en contextos empresariales o de investigación reales.

### **Importancia de la Práctica con Proyectos Reales**

Los ejercicios prácticos y los proyectos finales son indispensables para aplicar los conocimientos adquiridos y consolidar el aprendizaje.21 La creación y actualización de un portafolio con proyectos y certificaciones es clave para atraer la atención de empresas y demostrar la capacidad de resolver problemas de negocio utilizando el conocimiento obtenido de los datos.10

### **Participación en Comunidades y Recursos Adicionales**

Unirse a foros de discusión en plataformas de cursos o redes sociales permite resolver dudas, compartir aprendizajes y beneficiarse de la experiencia colectiva.21 La comunidad de R, por ejemplo, es entusiasta y comprometida, ofreciendo valiosos consejos y soluciones.22 Mantenerse al día sobre las innovaciones en el campo de la ciencia de datos es un imperativo, dado su rápido avance.10

### **Desarrollo de Habilidades de Comunicación**

Un científico de datos debe poseer sólidas habilidades comunicativas para transmitir claramente los resultados a los diferentes *stakeholders*, quienes a menudo no tienen un perfil técnico.10 La capacidad de convertir los datos en narrativas que estimulen la acción y creen valor es una habilidad diferenciadora.23  
El aprendizaje continuo y la adaptabilidad son imperativos en un campo en constante evolución. La ciencia de datos es un dominio dinámico donde nuevas técnicas, herramientas y desafíos emergen constantemente. Un científico de datos debe comprometerse con el aprendizaje a lo largo de toda su carrera, no solo para mantenerse relevante, sino para innovar y abordar problemas emergentes de manera efectiva. Esto implica una actitud proactiva hacia la exploración de nuevas metodologías y la revisión constante de los fundamentos.

## **Conclusiones**

Dominar la probabilidad y la estadística es indispensable para cualquier aspirante a científico de datos. Esta hoja de ruta subraya que no se trata solo de adquirir conocimientos teóricos, sino de desarrollar una profunda comprensión conceptual y la capacidad de aplicar estos principios en escenarios del mundo real. La interconexión entre probabilidad y estadística, junto con una base sólida en Álgebra Lineal y Cálculo, forma el andamiaje sobre el cual se construyen los modelos de datos más sofisticados y las decisiones más informadas.  
La elección de herramientas como Python o R debe ser estratégica, reconociendo las fortalezas complementarias de cada uno. Además, la participación activa en el aprendizaje a través de proyectos prácticos y la interacción con comunidades son tan cruciales como el estudio formal. Finalmente, la capacidad de comunicar hallazgos complejos de manera clara y concisa es lo que transforma el conocimiento técnico en valor empresarial. Al seguir esta hoja de ruta, los estudiantes no solo construirán una base técnica sólida, sino que también cultivarán la mentalidad y las habilidades necesarias para prosperar como científicos de datos en un entorno impulsado por los datos.

#### **Works cited**

1. es.khanacademy.org, accessed July 4, 2025, [https://es.khanacademy.org/math/probability/probability-geometry/probability-basics/a/probability-the-basics\#:\~:text=La%20probabilidad%20es%20simplemente%20qu%C3%A9,probabilidad%20se%20le%20llama%20estad%C3%ADstica.](https://es.khanacademy.org/math/probability/probability-geometry/probability-basics/a/probability-the-basics#:~:text=La%20probabilidad%20es%20simplemente%20qu%C3%A9,probabilidad%20se%20le%20llama%20estad%C3%ADstica.)  
2. Probabilidad: conceptos básicos (artículo) \- Khan Academy, accessed July 4, 2025, [https://es.khanacademy.org/math/probability/probability-geometry/probability-basics/a/probability-the-basics](https://es.khanacademy.org/math/probability/probability-geometry/probability-basics/a/probability-the-basics)  
3. Aprende sobre probabilidades con cursos online \- edX, accessed July 4, 2025, [https://www.edx.org/es/aprende/probabilidades](https://www.edx.org/es/aprende/probabilidades)  
4. Aprende las bases matemáticas para data science \- Platzi, accessed July 4, 2025, [https://platzi.com/blog/fundamentos-matematicas-data-science/](https://platzi.com/blog/fundamentos-matematicas-data-science/)  
5. Probabilidad y Estadística con Python \- Raul E. Lopez Briega, accessed July 4, 2025, [https://relopezbriega.github.io/blog/2015/06/27/probabilidad-y-estadistica-con-python/](https://relopezbriega.github.io/blog/2015/06/27/probabilidad-y-estadistica-con-python/)  
6. Probabilidad y estadística en el análisis de datos \- DbaExperts, accessed July 4, 2025, [https://dbaexperts.tech/database/probabilidad-y-estadistica/](https://dbaexperts.tech/database/probabilidad-y-estadistica/)  
7. Estadística descriptiva e inferencial en el análisis de datos \- Cognodata, accessed July 4, 2025, [https://www.cognodata.com/blog/estadistica-descriptiva-e-inferencial-analisis-datos/](https://www.cognodata.com/blog/estadistica-descriptiva-e-inferencial-analisis-datos/)  
8. ¿Qué es estadística descriptiva y estadística inferencial? \- Minitab \- Support, accessed July 4, 2025, [https://support.minitab.com/es-mx/minitab/help-and-how-to/statistics/basic-statistics/supporting-topics/basics/what-are-descriptive-and-inferential-statistics/](https://support.minitab.com/es-mx/minitab/help-and-how-to/statistics/basic-statistics/supporting-topics/basics/what-are-descriptive-and-inferential-statistics/)  
9. URosarioX: Probabilidad y estadística | edX, accessed July 4, 2025, [https://www.edx.org/learn/probability/universidad-del-rosario-probabilidad-y-estadistica](https://www.edx.org/learn/probability/universidad-del-rosario-probabilidad-y-estadistica)  
10. Científico de datos o data scientist: funciones y requisitos \- UNIR, accessed July 4, 2025, [https://www.unir.net/revista/ingenieria/cientifico-de-datos/](https://www.unir.net/revista/ingenieria/cientifico-de-datos/)  
11. Qué se NECESITA saber de MATEMÁTICA en CIENCIA DE DATOS | Mitos y consejos, accessed July 4, 2025, [https://www.youtube.com/watch?v=QPsOrOnQxvE](https://www.youtube.com/watch?v=QPsOrOnQxvE)  
12. Respuestas de Flexi \- ¿Cómo se utiliza el álgebra lineal en la ..., accessed July 4, 2025, [https://www.ck12.org/flexi/es/algebra/interpolacion-y-extrapolacion-lineal/como-se-utiliza-el-algebra-lineal-en-la-ciencia-de-datos/](https://www.ck12.org/flexi/es/algebra/interpolacion-y-extrapolacion-lineal/como-se-utiliza-el-algebra-lineal-en-la-ciencia-de-datos/)  
13. 4\. Álgebra lineal \- Ciencia de datos desde cero, 2ª edición \[Book\] \- O'Reilly Media, accessed July 4, 2025, [https://www.oreilly.com/library/view/ciencia-de-datos/9781098182625/ch04.html](https://www.oreilly.com/library/view/ciencia-de-datos/9781098182625/ch04.html)  
14. Las Matemáticas detrás de la Ciencia de Datos \- Blog de Código Facilito, accessed July 4, 2025, [https://codigofacilito.com/articulos/matematicas-ciencia-datos](https://codigofacilito.com/articulos/matematicas-ciencia-datos)  
15. Qué es una distribución de probabilidad \- DecisionesConDatos.com, accessed July 4, 2025, [https://www.decisionescondatos.com/que-es-una-distribucion-de-probabilidad](https://www.decisionescondatos.com/que-es-una-distribucion-de-probabilidad)  
16. Aprende sobre estadística con cursos online | edX, accessed July 4, 2025, [https://www.edx.org/es/aprende/estadistica](https://www.edx.org/es/aprende/estadistica)  
17. Estadística y probabilidad | Coursera, accessed July 4, 2025, [https://www.coursera.org/learn/estadistica-probabilidad](https://www.coursera.org/learn/estadistica-probabilidad)  
18. Distribución de probabilidad \- Wikipedia, la enciclopedia libre, accessed July 4, 2025, [https://es.wikipedia.org/wiki/Distribuci%C3%B3n\_de\_probabilidad](https://es.wikipedia.org/wiki/Distribuci%C3%B3n_de_probabilidad)  
19. Calcular probabilidades a partir de datos en Python \[2025\] \- KeepCoding, accessed July 4, 2025, [https://keepcoding.io/blog/calcular-probabilidades-datos-python/](https://keepcoding.io/blog/calcular-probabilidades-datos-python/)  
20. Probabilidad y estadística para la ciencia de datos \- Educación Continua Uniandes, accessed July 4, 2025, [https://educacioncontinua.uniandes.edu.co/probabilidad-y-estadistica-para-la-ciencia-de-datos/p](https://educacioncontinua.uniandes.edu.co/probabilidad-y-estadistica-para-la-ciencia-de-datos/p)  
21. MOOC Data Science: Inicia tu Carrera en Ciencia de Datos \- Aprender BIG DATA, accessed July 4, 2025, [https://aprenderbigdata.com/mooc-data-science/](https://aprenderbigdata.com/mooc-data-science/)  
22. Python vs. R: ¿cuál es mejor para la ciencia de datos? \- IONOS, accessed July 4, 2025, [https://www.ionos.com/es-us/digitalguide/paginas-web/desarrollo-web/python-vs-r/](https://www.ionos.com/es-us/digitalguide/paginas-web/desarrollo-web/python-vs-r/)  
23. Data Science para Negocios \- Certificado \- The University of Chicago, accessed July 4, 2025, [https://online.professional.uchicago.edu/es/certificado/certificado-en-data-science/](https://online.professional.uchicago.edu/es/certificado/certificado-en-data-science/)  
24. Matriz de covarianza \- Wikipedia, la enciclopedia libre, accessed July 4, 2025, [https://es.wikipedia.org/wiki/Matriz\_de\_covarianza](https://es.wikipedia.org/wiki/Matriz_de_covarianza)  
25. fastercapital.com, accessed July 4, 2025, [https://fastercapital.com/es/tema/interpretaci%C3%B3n-de-la-matriz-de-covarianza.html/1\#:\~:text=La%20matriz%20de%20covarianza%20es%20una%20matriz%20cuadrada%20que%20resume,de%20las%20relaciones%20entre%20variables.](https://fastercapital.com/es/tema/interpretaci%C3%B3n-de-la-matriz-de-covarianza.html/1#:~:text=La%20matriz%20de%20covarianza%20es%20una%20matriz%20cuadrada%20que%20resume,de%20las%20relaciones%20entre%20variables.)  
26. Autovalores y autovectores en ML | KeepCoding Bootcamps, accessed July 4, 2025, [https://keepcoding.io/blog/autovalores-y-autovectores-en-ml/](https://keepcoding.io/blog/autovalores-y-autovectores-en-ml/)  
27. 31\. Reducción de dimensionalidad con PCA — Computación Científica con Python, accessed July 4, 2025, [https://phuijse.github.io/PythonBook/contents/sklearn/pca.html](https://phuijse.github.io/PythonBook/contents/sklearn/pca.html)  
28. Autovectores: ¡otro inútil capricho de los matemáticos\! \- Ciencia explicada, accessed July 4, 2025, [https://www.ciencia-explicada.com/2012/01/autovectores-otro-inutil-capricho-de.html](https://www.ciencia-explicada.com/2012/01/autovectores-otro-inutil-capricho-de.html)  
29. fastercapital.com, accessed July 4, 2025, [https://fastercapital.com/es/contenido/Descomposicion-de-valores-singulares--SVD--Descomposicion-de-datos--una-inmersion-en-la-descomposicion-de-valores-singulares.html\#:\~:text=La%20descomposici%C3%B3n%20de%20valores%20singulares%20(SVD)%20es%20una%20t%C3%A9cnica%20poderosa,exenta%20de%20desaf%C3%ADos%20y%20consideraciones.](https://fastercapital.com/es/contenido/Descomposicion-de-valores-singulares--SVD--Descomposicion-de-datos--una-inmersion-en-la-descomposicion-de-valores-singulares.html#:~:text=La%20descomposici%C3%B3n%20de%20valores%20singulares%20\(SVD\)%20es%20una%20t%C3%A9cnica%20poderosa,exenta%20de%20desaf%C3%ADos%20y%20consideraciones.)  
30. Descomposición en valores singulares y análisis de factores en ciencias humanas y sociales Singular Value Decomposition and fa \- UPO, accessed July 4, 2025, [https://www.upo.es/revistas/index.php/RevMetCuant/article/download/8004/8441/40259](https://www.upo.es/revistas/index.php/RevMetCuant/article/download/8004/8441/40259)  
31. OPTIMIZACIÓN CONVEXA EN CIENCIA DE DATOS \- UNED, accessed July 4, 2025, [https://www.uned.es/universidad/inicio/en/estudios/masteres/master-universitario-en-matematicas-avanzadas/asignaturas.html?codAsignatura=21520086\&codTitulacion=215201\&idContenido=1](https://www.uned.es/universidad/inicio/en/estudios/masteres/master-universitario-en-matematicas-avanzadas/asignaturas.html?codAsignatura=21520086&codTitulacion=215201&idContenido=1)  
32. Qué es: Optimización convexa \- Aprenda estadísticas fácilmente, accessed July 4, 2025, [https://es.statisticseasily.com/glossario/what-is-convex-optimization-detailed-overview/](https://es.statisticseasily.com/glossario/what-is-convex-optimization-detailed-overview/)  
33. Tipos de gráficos para Data Science y Data Analytics: Guía Práctica \- ID Bootcamps, accessed July 4, 2025, [https://iddigitalschool.com/bootcamps/tipos-de-graficos-para-data-science-y-data-analytics-guia-practica/](https://iddigitalschool.com/bootcamps/tipos-de-graficos-para-data-science-y-data-analytics-guia-practica/)  
34. Los tipos de gráficos estadísticos \- INE, accessed July 4, 2025, [https://www.ine.es/explica/docs/pasos\_tipos\_graficos.pdf](https://www.ine.es/explica/docs/pasos_tipos_graficos.pdf)  
35. \#Bayes' \#Theorem 004 Fundamentals of \#DataScience \- YouTube, accessed July 4, 2025, [https://www.youtube.com/watch?v=YMxDbqMzGsI](https://www.youtube.com/watch?v=YMxDbqMzGsI)  
36. Qué es el Teorema de Bayes y qué importancia tiene en Machine Learning \- Kraz Blog, accessed July 4, 2025, [https://blog.kraz.ai/marketing/que-es-el-teorema-de-bayes-y-que-importancia-tiene-en-machine-learning/](https://blog.kraz.ai/marketing/que-es-el-teorema-de-bayes-y-que-importancia-tiene-en-machine-learning/)  
37. www.jove.com, accessed July 4, 2025, [https://www.jove.com/es/science-education/v/16480/accuracy-and-errors-in-hypothesis-testing\#:\~:text=Un%20error%20de%20Tipo%20I,establece%20com%C3%BAnmente%20en%200%2C05.](https://www.jove.com/es/science-education/v/16480/accuracy-and-errors-in-hypothesis-testing#:~:text=Un%20error%20de%20Tipo%20I,establece%20com%C3%BAnmente%20en%200%2C05.)  
38. INFERENCIA ESTADÍSTICA: PRUEBAS DE HIPÓTESIS \- Revista Chilena de Anestesia, accessed July 4, 2025, [https://revistachilenadeanestesia.cl/inferencia-estadistica-pruebas-de-hipotesis/](https://revistachilenadeanestesia.cl/inferencia-estadistica-pruebas-de-hipotesis/)  
39. ¿Qué es la regresión logística? \- Explicación del modelo de regresión logística \- AWS, accessed July 4, 2025, [https://aws.amazon.com/es/what-is/logistic-regression/](https://aws.amazon.com/es/what-is/logistic-regression/)  
40. Regresión logística Python \- cienciadedatos.net, accessed July 4, 2025, [https://cienciadedatos.net/documentos/py17-regresion-logistica-python](https://cienciadedatos.net/documentos/py17-regresion-logistica-python)  
41. Métricas de evaluación de modelos de regresión \- Dialéktico, accessed July 4, 2025, [https://dialektico.com/metricas-de-evaluacion-de-modelos-de-regresion/](https://dialektico.com/metricas-de-evaluacion-de-modelos-de-regresion/)  
42. Métricas en regresión. La regresión es importante y conocer… | by Nicolás Arrioja Landa Cosio | Medium, accessed July 4, 2025, [https://medium.com/@nicolasarrioja/m%C3%A9tricas-en-regresi%C3%B3n-5e5d4259430b](https://medium.com/@nicolasarrioja/m%C3%A9tricas-en-regresi%C3%B3n-5e5d4259430b)  
43. Machine Learning: Seleccion Métricas de clasificación \- sitiobigdata.com, accessed July 4, 2025, [https://sitiobigdata.com/2019/01/19/machine-learning-metrica-clasificacion-parte-3/](https://sitiobigdata.com/2019/01/19/machine-learning-metrica-clasificacion-parte-3/)  
44. ¿Qué es la agrupación en clústeres k-means? \- IBM, accessed July 4, 2025, [https://www.ibm.com/mx-es/think/topics/k-means-clustering](https://www.ibm.com/mx-es/think/topics/k-means-clustering)  
45. K-means (o K-medias) para detección de Clusters: Algoritmo e implementación con Python, accessed July 4, 2025, [https://www.youtube.com/watch?v=mICySHB0fh4](https://www.youtube.com/watch?v=mICySHB0fh4)