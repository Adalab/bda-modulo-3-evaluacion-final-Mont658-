# ✈️ Análisis de Clientes de una aerolinea

Este repositorio contiene el trabajo realizado como parte de la **evaluación final del Módulo 3** del bootcamp de **Data Analytics en Adalab**. El objetivo ha sido aplicar de forma integrada todo lo aprendido sobre limpieza, análisis y visualización de datos reales.

---

## 🧠 Lo que he hecho paso a paso

### 🔍 Exploración inicial

* Carga de los dos CSV y revisión con `eda_basico()` para entender el contenido.
* Búsqueda de duplicados, columnas constantes y valores nulos.

### 🧼 Limpieza de datos

* Eliminación de columnas irrelevantes como `Country`.
* Reemplazo de nulos en:

  * `Salary`: primero corregí los valores negativos, y luego imputé los nulos con SimpleImputer.
  * `Cancellation Month`: convertí los nulos en 'No'.
* Conversión de columnas de mes numérico a nombre en inglés como variable categórica ordenada.

### 🔗 Unificación de datos

* Realicé un `merge` por `Loyalty Number` para tener la información combinada de actividad y perfil.

### 🕓 Preparación de fechas

* Transformé `Enrollment Year` y `Cancellation Year` a tipo fecha (solo año).
* Los meses los mantuve como categorías (por nombre, no número).
* Creamos `Registration Date` para facilitar análisis temporales.

---

## 📊 Visualizaciones realizadas

1. **Vuelos reservados por mes**: línea temporal con promedio mensual.
2. **Distancia vs Puntos acumulados**: scatterplot con relación muy clara y lineal.
3. **Salario por nivel educativo**: barplot usando la media.
4. **Distribución por tipo de tarjeta**: gráfico circular y de barras.
5. **Distribución por género y estado civil**: countplot mejorado con `hue`, cambiando el eje X para que se vea más claro.

---

## 📌 Conclusiones personales

* Las visualizaciones ayudan mucho a detectar patrones y relaciones lógicas.
* Aprendí a limpiar datos no solo con funciones sueltas, sino con criterio.
* Añadir categorías, convertir fechas, y adaptar los gráficos fueron claves.
* Lo que más me costó fue combinar datos reales, pero también fue lo más satisfactorio.

---

## ✅ Herramientas y buenas prácticas

* Python, Pandas, Matplotlib, Seaborn, scikit-learn (KNNImputer)
* Código comentado y modular (funciones separadas por tarea)

---

*Gracias por revisar mi trabajo. Ha sido un reto y también un logro.*
