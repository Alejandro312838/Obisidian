La máxima verosimilitud (Maximum Likelihood) es un ==método estadístico utilizado para estimar los parámetros de un modelo==. En esencia, busca los valores de los parámetros que hacen que los datos observados sean lo más probables posible. Se utiliza en una variedad de campos, incluyendo la estadística, el aprendizaje automático y la bioinformática. 

##### **siempre parte del supuesto de que los datos provienen de una distribución definida**.

En términos más simples:
1. **1.** **Función de Verosimilitud:**
    Se define una función que describe la probabilidad de observar los datos que tenemos, dado un conjunto específico de valores para los parámetros del modelo. 
    
- **2.** **Maximización:**
    El objetivo es encontrar los valores de los parámetros que maximizan esta función de verosimilitud. Estos valores son considerados la estimación de máxima verosimilitud. 
    
- **3.** **Interpretación:**
    
    La estimación de máxima verosimilitud nos da los valores de los parámetros que mejor explican los datos observados, según el modelo elegido

![[Pasted image 20250717164731.png]]
Debemos encontrar la funcion de prob azul (pues es donde los valores son mas probables) o bien, debemos de estimar los parametros de la muestra morada (como este caso es una distribucion normal entonces debemos de encontrar su media y su desviacion estandar)

The true distribution from which the data were generated was f1 ~ N(10, 2.25), which is the blue curve in the figure above.

# 📊 Máxima Verosimilitud (MLE)

## 🧩 ¿Qué es la MLE?
La **Máxima Verosimilitud (MLE)** es un método para estimar parámetros desconocidos de una población. Busca los valores de los parámetros que **hacen más probable haber observado la muestra que tenemos**.

---

## 🧮 Pasos para encontrar la función de verosimilitud

1. **Identificar la distribución de la muestra**  
   Asume que los datos provienen de una distribución conocida (ej. normal, exponencial, binomial, etc.).

2. **Escribir la función de densidad o probabilidad**  
   Escribe \( f(x_i; \theta) \), la función de probabilidad o densidad para una sola observación, en función del parámetro desconocido \( \theta \).

3. **Construir la función de verosimilitud**  
   Si la muestra es \( x_1, x_2, ..., x_n \), entonces:
$$
   L(\theta) = \prod_{i=1}^{n} f(x_i; \theta)
   $$
   

5. **Tomar logaritmo (opcional pero recomendado)**  
   Para simplificar, se suele usar la log-verosimilitud:

   \[$$
   \log L(\theta) = \sum_{i=1}^{n} \log f(x_i; \theta)
   $$

6. **Derivar e igualar a cero**  
   Deriva respecto al parámetro \( \theta \), y resuelve \( \frac{d}{d\theta} \log L(\theta) = 0 \).

7. **Verificar que es un máximo**  
   Usa la segunda derivada o analiza el comportamiento de la función para confirmar que encontraste un máximo.

---

## 📌 Notas importantes

### ✅ La MLE tiene **una forma fija para cada distribución**

- Por ejemplo, si los datos vienen de una **normal con varianza conocida**, la MLE de la media \( \mu \) **siempre será** el promedio muestral:
  
  \[$$
  \hat{\mu} = \frac{1}{n} \sum x_i
  $$

- Si los datos vienen de una **exponencial**, la MLE del parámetro \( \lambda \) será:

  $$
  \hat{\lambda} = \frac{n}{\sum x_i} = \frac{1}{\bar{x}}
  $$

> ✨ *Es decir, la fórmula del estimador es fija para cada tipo de distribución. Lo que cambia con la muestra es el valor numérico del estimador, no la forma general.*

---

### ❓ ¿Qué pasa si **no se conoce la distribución**?

Si la distribución de la población **no está bien definida** o **no quieres asumir una forma específica**, **no puedes usar MLE tradicional**. En ese caso puedes:

- Usar una **distribución aproximada** si tiene sentido (modelo paramétrico).
- Usar **métodos no paramétricos** (como histogramas, estimadores kernel, bootstrap).
- Usar modelos **semi-paramétricos**, donde partes del modelo son conocidos y otras no.

> ⚠️ *La MLE requiere una función de densidad conocida. Si no puedes definirla, necesitas técnicas alternativas.*

---

## 🧠 Resumen

- La MLE busca el parámetro que maximiza la probabilidad de observar la muestra.
- Cada distribución tiene una **fórmula MLE fija**.
- Si no conoces la distribución, debes usar métodos **no paramétricos o semi-paramétricos**.


