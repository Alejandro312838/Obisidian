# 🧪 Conceptos de Pruebas de Hipótesis

Las **pruebas de hipótesis** son procedimientos estadísticos que permiten tomar decisiones sobre una población, basándose en los datos de una muestra. Su objetivo es evaluar si una afirmación sobre un parámetro poblacional es razonable o no, dados los datos observados.

---

## 📌 Conceptos Fundamentales

### 🔸 Hipótesis nula (H0)
Es la afirmación que se somete a prueba. Generalmente representa el estado actual, ausencia de efecto o igualdad.

**Ejemplo:** H0: la media es igual a 100

### 🔸 Hipótesis alternativa (H1 o Ha)
Es la afirmación opuesta a H0. Representa el efecto, diferencia o cambio que se desea detectar.

**Ejemplo:** H1: la media es diferente de 100

---

## 📊 Tipos de prueba

### 🔹 Prueba unilateral (una cola)
Se utiliza cuando se quiere detectar un cambio en una sola dirección.

- H1: la media es mayor que cierto valor
- H1: la media es menor que cierto valor

### 🔹 Prueba bilateral (dos colas)
Se utiliza cuando se busca detectar cualquier cambio, ya sea mayor o menor.

- H1: la media es diferente (mayor o menor)

---

## 🧮 Estadístico de prueba

Es un valor que se calcula a partir de la muestra para decidir si se rechaza o no H0.  
Ejemplos de estadísticos: Z, t, chi-cuadrado, F, etc.

La fórmula depende del tipo de prueba y si se conoce o no la desviación estándar poblacional.

---

## 📈 Nivel de significancia (alpha)

Es la probabilidad de cometer un error tipo I (rechazar H0 cuando en realidad es verdadera).  
Valores comunes: 0.05, 0.01, 0.10

---

## 📉 Valor-p (p-value)

Es la probabilidad de obtener un resultado igual o más extremo que el observado, **suponiendo que H0 es verdadera**.

- Si **p ≤ alpha**, se **rechaza H0**
- Si **p > alpha**, **no se rechaza H0**

---

## ❗ Tipos de errores

### 🔸 Error tipo I
- Ocurre cuando se rechaza H0 siendo verdadera.
- Probabilidad: alpha

### 🔸 Error tipo II
- Ocurre cuando no se rechaza H0 siendo falsa.
- Probabilidad: beta

### 🔸 Potencia de la prueba
- Es la probabilidad de rechazar H0 cuando realmente es falsa.
- Se calcula como 1 - beta

---

## 🧠 Otros conceptos importantes

### 🔹 Región crítica o de rechazo
Conjunto de valores del estadístico para los cuales se rechaza H0.

### 🔹 Región de aceptación
Valores del estadístico para los cuales no se rechaza H0.

### 🔹 Tipo de prueba estadística
- Prueba Z: para medias con desviación estándar conocida
- Prueba t: para medias con desviación estándar desconocida
- Prueba chi-cuadrado: para varianzas o tablas de frecuencia
- Prueba F: para comparar varianzas entre dos poblaciones

---

## ✅ Pasos para realizar una prueba de hipótesis

1. Plantear las hipótesis H0 y H1
2. Elegir el nivel de significancia (alpha)
3. Seleccionar el estadístico adecuado
4. Calcular el valor del estadístico con los datos muestrales
5. Determinar la región crítica o calcular el p-value
6. Tomar una decisión:
   - Si el valor cae en la región crítica o p ≤ alpha → Rechazar H0
   - Si no cae en la región crítica o p > alpha → No rechazar H0

---

## 📚 Ejemplos comunes de pruebas

- Prueba para una media: H0: media = valor específico
- Prueba para una proporción: H0: proporción = valor específico
- Prueba para una varianza: H0: varianza = valor específico
- Comparación de dos medias: H0: media1 = media2
- Prueba de independencia en tablas de contingencia

