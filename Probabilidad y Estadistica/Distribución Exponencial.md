La distribución exponencial es una distribución de probabilidad continua que modela el tiempo entre sucesos en un proceso en el que los sucesos ocurren de forma continua e independiente a una tasa media constante. Es especialmente útil para analizar situaciones que implican tiempos de espera, tiempos de vida e intervalos entre sucesos.
Responde a las preguntas
"Para hallar la probabilidad de esperar entre X y Y minutos a la siguiente acción"
"¿Cuál es la probabilidad de que recibamos una acción en los primeros X minutos?"
#### Función de densidad de probabilidad (PDF)

**La PDF nos ayuda a calcular la probabilidad de que se produzca un suceso en un intervalo determinado. La PDF de la distribución exponencial es la siguiente:**
![[Pasted image 20250709151319.png]]
   donde:
- x es la variable aleatoria (normalmente representa el tiempo)
- λ es el parámetro de la tasa (λ > 0)
- e es el número de Euler (aproximadamente 2,71828)

#### Función de distribución acumulativa (FDA)

**La FCD es especialmente útil cuando queremos hallar la probabilidad de que un suceso ocurra antes de un tiempo determinado. Nos da la probabilidad de que el tiempo de espera sea menor o igual que un valor determinado. Aquí tienes la FDA de la distribución exponencial:**
![[Pasted image 20250709151337.png]]

Ejemplo
Imagina que estamos analizando las llamadas de atención al cliente en un servicio de asistencia, donde las llamadas llegan siguiendo una distribución exponencial con una tasa media de 3 llamadas por hora (λ = 3).

Para hallar la probabilidad de esperar entre 10 y 20 minutos a la siguiente llamada, haríamos:

1. **Convierte el tiempo en horas:** (10 minutos = 1/6 de hora, 20 minutos = 1/3 de hora)
2. **Utiliza la fórmula**: P(1/6 < X < 1/3) = ∫[1/6 a 1/3] 3e^(-3x)dx
3. **Evalúa**: = -e^(-3x)|[1/6 a 1/3]
4. **Calcula**: = [e(-0,5) - e(-1)] ≈ 0,2325 o aproximadamente 23,25%.

Ahora, ¿Cuál es la probabilidad de que recibamos una llamada en los primeros 15 minutos?
1. **Convierte 15 minutos en horas:** (15 minutos = 1/4 de hora)
2. **Utiliza la fórmula CDF**: F(1/4) = 1 - e^(-3x1/4)
3. **Calcula**: = 1 - e^(-0,75) ≈ 0,5276 o alrededor del 52,76%.