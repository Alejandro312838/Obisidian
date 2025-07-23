Distribución a priori: Representa lo que creemos sobre un parámetro antes de ver los datos.
	Ejemplo: No sabemos si una moneda está cargada (no sea 50-50) pero cómo no la hemos lanzado aún entonces asumimos que es justa
Distribución a Posteriori: Es nuestra nueva creencia actualizada después de ver los datos o realizar un experimento.
	Ejemplo: Lanzamos la moneda 5 veces y vemos que cayó 4 veces cara y 1 vez cruz, por lo que nuestra creencia actualizada es que la moneda 	probablemente está cargada
Verosimilitud: La verosimilitud es una forma de medir qué tan compatibles son los datos que observaste con una hipótesis concreta.
	Imagina que ocurrió un crimen y tienes 3 sospechosos:
    Sospechoso A: Estaba en la escena y tiene un motivo.
    Sospechoso B: Vive en otro país.
    Sospechoso C: No tiene coartada.
🔍 Luego encuentras una huella digital.
Preguntas: “Si el sospechoso A fuera el culpable, ¿qué tan probable es esta huella?” → alta verosimilitud
Ahora con el sospechoso B (que vive lejos), dices: “Si él fuera el culpable, ¿es probable que deje esta huella aquí?” → baja verosimilitud
Inferencia Bayeisiana: ![[Pasted image 20250622180103.png]]![[Pasted image 20250622180134.png]]


Supón esto:

- Sabes que en una fiesta hay **10 pasteles**.
    
- Uno de ellos **podría estar envenenado**.
    
- Antes de ver nada, piensas que **todos tienen la misma probabilidad** de estar envenenado: eso es tu **prior** (creencia previa).
Método Monte Carlo: La simulación de Monte Carlo es un tipo de algoritmo computacional que utiliza muestreo aleatorio repetido para obtener la probabilidad de que se produzca un rango de resultados.
	Ejemplo: No sabemos el valor de pi y queremos aproximarlo
	Creamos la siguiente figura
	![[Pasted image 20250621203249.png]]
	Sabemos que el area del circulo es piR^2
	El area del cuadrado es 4R^2
	Por lo tanto tenemos que circulo/cuadrado  (proporcion)= pi/4
	Con un generador de numeros aleatorios generamos coordenadas dentro del espacio y llevamos cuenta de cuántos puntos quedan dentro y fuera del círculo
	Si generamos 100 puntos y tenemos que 81 cayeron dentro del circulo y 19 no
	Por lo tanto 81/100 = pi / 4;  pi = (81x4)/100 = 3.24
	El error de este metodo es Raiz de n donde n es el numero de veces que hacemos el experimento
![[Pasted image 20250622152918.png]]
Muestreo por rechazo (aceptacion-rechazo)
	técnica utilizada para generar muestras aleatorias de una distribución objetivo, especialmente cuando es difícil o imposible muestrear directamente de ella
	Proponemos g(s) que es una distribucion mucho mas sencilla que f(s) y que ademas se acerca a esta ultima
	![[Pasted image 20250621213543.png]]
	Escalamos g(s) por M para que este por encima de f(s) (asi tambien aseguramos que el resultado siempre va a estar en rango 0 a 1)
	![[Pasted image 20250621213734.png]]
	Para saber si aceptamos o no una muestra seguimos lo siguiente que nos va a dar una probabilidad 0-100%, nosotros decidimos el umbral
	![[Pasted image 20250621214602.png]]
	aclaraciones: Conocer una función de distribución solo te permite calcular la probabilidad de una muestra. Generar muestras a partir de esa función es una tarea diferente.
	Ejemplo: Sabes que una variable sigue una **distribución normal**:
	![[Pasted image 20250621214715.png]]
	Eso significa que **puedes calcular** cosas como:
- ¿Cuál es la probabilidad de que xxx esté entre -1 y 1?
- ¿Cuál es la densidad en x=0.5x = 0.5x=0.5? (Es decir, f(0.5)f(0.5)f(0.5))
- Ahora imagina que quieres hacer una simulación y necesitas **números aleatorios que se comporten como si vinieran de esa distribución normal**.
🔁 Aquí no basta con conocer la fórmula. Necesitas **un proceso (algoritmo)** que genere esos valores.
🎲 Por ejemplo:
- Un generador que te dé números como: -0.8, 0.3, 1.2, -1.4, etc., **siguiendo la forma de la curva normal**.
- Esos números deben salir con más frecuencia donde la curva es más alta, y menos donde es baja.
	Desventajas del muestreo por rechazo: es dificil encontrar un g(s) que sea simple y que a la vez se parezca a la funcion
	![[Pasted image 20250621214921.png]]
	Este metodo no tiene memoria, por lo que si encontramos un valor que es muy probable en f(x) deberiamos de generar mas numeros por ese rango, sin embargo el metodo sigue generando numeros aleatorios sin ningun bias, aqui es donde el metodo MCMC entra

Muestreo Monte Carlo por cadenas de Markov (MCMC - Metropolis Hastings):
	Cadenas de Márkov: modelo matemático que describe una secuencia de eventos donde la probabilidad de que ocurra un evento depende únicamente del estado inmediatamente anterior
		Ejemplo: En un restaurante te dan la carta y puedes elegir entre carne, cerdo o pescado	
		después de elegir, te dan a elegir entre 3 bebidas, vino tino, cerveza, refresco
		La selección de la bebida depende de que elegiste para comer
		
	El metodo: el siguiente muestreo depende del ultimo
	Distribucion estacionaria: propiedad de las cadenas de Markov, dice que si la cadena llega a esta distribucion entonces se va a quedar en esa distribucion por el resto de las muestras "a probability distribution that remains unchanged over time as the chain evolves"
	Entonces, lo que queremos es diseñar una cadena de markov cuya distribución estacionaria sea nuestra f(x) )(nuestra distribución target de la que queremos sacar muestras)
	Comenzamos en un punto "a" al azar y proponemos el punto "b", si f(b) > f(a) entonces T(a->b) = 1 (100%)
	en caso contrario, la prob de aceptar esa propuesta de punto "b" es f(b) / f(b) esto porque queremos aun asi sacar muestras de la cola de la distribucion, si no hacemos esto, nos quedariamos atrapados en un solo punto

### Usos en simulaciones

## 1. 🟢 **Monte Carlo directo**

### 🎲 Simular la probabilidad de que al menos dos personas compartan cumpleaños en un grupo (el famoso "problema del cumpleaños")

---

### 🧠 ¿Qué queremos hacer?

Queremos saber:

> “¿Cuál es la probabilidad de que en un grupo de 23 personas, al menos dos cumplan años el mismo día?”

Este cálculo exacto es difícil manualmente, pero se puede hacer fácilmente por simulación.

---

### 👟 Cómo lo hacemos (Monte Carlo):

1. Simulamos 10,000 grupos de 23 personas.
    
2. Para cada grupo, generamos un cumpleaños aleatorio (1–365) para cada persona.
    
3. Contamos cuántos grupos tienen **al menos una coincidencia**.
    

---

### 🤯 ¿Por qué es Monte Carlo?

Porque **podemos generar muestras directamente** de la distribución (cumpleaños al azar), sin necesidad de fórmulas complicadas.

---

### 🧁 Aplicación real:

Simular la probabilidad de colisiones en IDs generadas aleatoriamente (por ejemplo, en bases de datos, códigos QR, claves únicas).

---

## 2. 🔴 **Rechazo**

### 🚦 Control de calidad: detectar si una pieza es aceptable según su medida

---

### 🧠 ¿Qué queremos hacer?

Supón que fabricas tornillos, y **solo aceptas los que miden entre 19.8 mm y 20.2 mm**. La máquina produce tornillos con un tamaño entre 18 mm y 22 mm, distribuidos de forma desconocida.

No puedes generar tornillos **directamente dentro del rango aceptable**, pero puedes:

---

### 👟 Cómo lo haces (Rechazo):

1. Generas tornillos al azar entre 18 y 22 mm.
    
2. Si el tornillo está entre 19.8 y 20.2 mm → lo **aceptas**.
    
3. Si no, lo rechazas.
    

---

### 🤯 ¿Por qué es rechazo?

Porque estás **proponiendo valores de una distribución más amplia**, y **filtrando los que te interesan**.

---

### 🧁 Aplicación real:

Simulación de producción para saber **cuántas piezas necesitarás producir para tener suficientes dentro de especificaciones**, o estimar la tasa de desperdicio.

---

## 3. 🔁 **MCMC (Metropolis-Hastings)**

### 🏥 Estimar la prevalencia real de una enfermedad en una población

---

### 🧠 ¿Qué queremos hacer?

Tienes datos de pruebas médicas:

- La prueba tiene un **5% de falsos positivos** y un **2% de falsos negativos**.
    
- De 1,000 personas, 100 dieron positivo.
    

Quieres estimar:

> “¿Cuál es la proporción real de personas enfermas en la población?”

Este problema **tiene muchas fuentes de incertidumbre**, y es difícil calcular una distribución exacta.

---

### 👟 Cómo lo haces (MCMC):

1. Empiezas con una suposición: por ejemplo, 10% de personas enfermas.
    
2. Propones cambiarla un poco (por ejemplo, subir a 12%).
    
3. Evalúas si **con ese nuevo valor** los datos observados (100 positivos) serían más o menos probables.
    
4. Si el nuevo valor explica mejor los datos, lo aceptas.
    
5. Repites muchas veces y ves cómo se distribuyen tus hipótesis.
    

---

### 🤯 ¿Por qué es MCMC?

Porque **no puedes generar muestras directas**, ni aplicar rechazo eficientemente.  
Te mueves **paso a paso por el espacio de hipótesis**, generando una distribución realista de posibilidades.

---

### 🧁 Aplicación real:

Estimar tasas de enfermedades, fallos en sistemas de seguridad, proporción de votos ocultos, etc., **cuando los datos son ruidosos o indirectos**.

---

## 🗂️ RESUMEN DE LOS EJEMPLOS

|Método|Ejemplo real|Qué simula|Tipo de tarea|
|---|---|---|---|
|Monte Carlo|Probabilidad de compartir cumpleaños|Generar muestras directas para estimar una probabilidad|Simulación sencilla y directa|
|Rechazo|Control de calidad de tornillos|Filtrar valores buenos desde una distribución amplia|Cuando tienes una condición de corte|
|MCMC|Estimar proporción real de enfermos|Explorar hipótesis paso a paso según qué tan bien explican los datos|Para problemas con incertidumbre compleja|
