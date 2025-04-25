# Predicción del Rendimiento Académico de los Estudiantes

## Descripción

Este proyecto utiliza técnicas de aprendizaje automático para predecir el rendimiento académico de los estudiantes en función de diversas características. Se exploran dos modelos: Random Forest y Regresión Lineal.

## Datos

El conjunto de datos utilizado se obtuvo de Kaggle: [Student Study Performance](enlace al dataset en Kaggle). Contiene información sobre el rendimiento de los estudiantes en diferentes materias, junto con datos demográficos y académicos.

## Preprocesamiento de Datos

Se realizaron los siguientes pasos de preprocesamiento:

1. **Creación de la variable objetivo 'score'**: Se calculó el promedio de las calificaciones de las tres materias y se redondeó para crear la variable objetivo 'score'.
2. **Codificación One-Hot**: Se aplicó a las variables categóricas 'gender', 'race_ethnicity', 'lunch' y 'test_preparation_course'.
3. **Codificación Ordinal**: Se utilizó para la variable 'parental_level_of_education', estableciendo un orden jerárquico para los niveles de educación.

## Modelos de Aprendizaje Automático

Se entrenaron dos modelos de aprendizaje automático:

* **Random Forest**: Un modelo de conjunto que combina múltiples árboles de decisión.
* **Regresión Lineal**: Un modelo lineal que busca la relación entre las variables predictoras y la variable objetivo.

## Evaluación del Modelo

Se utilizó el error cuadrático medio (MSE) para evaluar el rendimiento de los modelos. Se dividieron los datos en conjuntos de entrenamiento y prueba para obtener una estimación precisa del rendimiento del modelo en datos no vistos.

## Resultados

Se obtuvieron los siguientes resultados para el MSE:

* Random Forest MSE: [inserta el valor del MSE de Random Forest]
* Linear Regression MSE: [inserta el valor del MSE de Regresión Lineal]

## Conclusiones

A pesar de la aplicación de técnicas de preprocesamiento y la utilización de dos modelos de aprendizaje automático diferentes, los resultados obtenidos en términos de MSE no fueron satisfactorios para la predicción del rendimiento académico de los estudiantes. Esto sugiere que:

* **Las variables predictoras utilizadas podrían no ser suficientemente informativas para explicar la variabilidad en el rendimiento académico.** Es posible que existan otros factores, como la motivación del estudiante, el entorno familiar, o la calidad de la enseñanza, que no se capturan en el conjunto de datos y que tienen un mayor impacto en el rendimiento.
* **Los modelos utilizados podrían no ser los más adecuados para este tipo de problema.** Se podrían explorar otros modelos de aprendizaje automático, como redes neuronales o máquinas de vectores de soporte, para ver si se obtiene un mejor rendimiento.
* **El conjunto de datos podría tener limitaciones, como un tamaño de muestra reducido o la presencia de ruido.** Sería beneficioso contar con un conjunto de datos más grande y representativo para entrenar los modelos.

**Futuras Direcciones:**

* **Incorporar nuevas variables predictoras:** Se podrían recopilar datos adicionales sobre los estudiantes, como su historial académico previo, sus hábitos de estudio, o su participación en actividades extracurriculares.
* **Experimentar con diferentes modelos de aprendizaje automático:** Se podrían probar otros modelos más complejos, como redes neuronales, para ver si se ajustan mejor a los datos.
* **Ajustar los hiperparámetros de los modelos:** Se podría realizar una búsqueda de hiperparámetros para optimizar el rendimiento de los modelos existentes.
* **Realizar un análisis más profundo de los datos:** Se podrían utilizar técnicas de análisis exploratorio de datos para identificar patrones y relaciones entre las variables que podrían ser relevantes para la predicción del rendimiento académico.

A pesar de los resultados obtenidos, este proyecto sirve como punto de partida para futuras investigaciones en la predicción del rendimiento académico. Se espera que las futuras mejoras en la selección de variables, los modelos de aprendizaje automático y el análisis de datos permitan obtener modelos más precisos y robustos.

## Instrucciones de Uso

1. Descarga el conjunto de datos de Kaggle.
2. Ejecuta el notebook de Colab paso a paso.
3. Ajusta los parámetros de los modelos si lo deseas.

## Dependencias

* pandas
* scikit-learn
* kagglehub
