# Detección de cáncer de mama mediante un enfoque estadístico, utilizando datos de la Universidad de Wisconsin con Statsmodels

## Introducción
En este proyecto, se exploró un enfoque estadístico utilizando datos de la Universidad de Wisconsin para predecir el diagnóstico de cáncer de mama. Se utilizó la biblioteca Statsmodels para construir y analizar un modelo de regresión logística que permite identificar patrones y factores de riesgo asociados con esta enfermedad. Este enfoque proporciona una comprensión profunda de los coeficientes y el impacto de las variables predictoras en los modelos estadísticos.

## Descripción del proyecto
El objetivo de este proyecto fue utilizar un enfoque estadístico para la detección de cáncer de mama. Se realizó una exploración exhaustiva de los datos, buscando valores perdidos y duplicados, y visualizando las correlaciones entre las variables predictoras mediante gráficos de pares (PairGrid) y mapas de calor. Basándose en estas correlaciones, se seleccionaron las variables más relevantes para construir el modelo de regresión logística. Los datos se dividieron en variables predictoras y variable respuesta, y se añadió un término constante a las variables predictoras. Posteriormente, se construyó y ajustó el modelo logístico, evaluando su rendimiento mediante matrices de confusión y métricas de exactitud, recall (sensibilidad) y F1-score.

## Características principales del proyecto
Exploración de datos: Análisis exhaustivo de los datos, incluyendo la búsqueda de valores perdidos y duplicados.
Visualización de correlaciones: Uso de gráficos de pares y mapas de calor para identificar correlaciones entre las variables predictoras.
Selección de variables: Selección de las variables más relevantes para el modelo de regresión logística.
Construcción y ajuste del modelo: Creación y ajuste de un modelo de regresión logística utilizando Statsmodels.
Evaluación del modelo: Análisis de matrices de confusión y métricas de rendimiento (exactitud, sensibilidad, F1-score).
División de datos: Separación de los datos en conjuntos de entrenamiento y prueba.

## Herramientas utilizadas
**Lenguaje de programación**: 
-	Python
**Librerías de Python**:
- Pandas (para manipulación de datos)
-	Numpy (para operaciones numéricas)
-	Matplotlib y seaborn (para visualización de datos)
-	Statsmodels (para análisis estadístico)
-	Scikit-learn (para preprocesamiento y evaluación de modelos)
-	Entorno de desarrollo: Jupyter Notebook
-	Dataset: Wisconsin Breast Cancer Dataset

## Conclusión
Al optimizar el modelo de regresión logística, se observó que se ajusta adecuadamente a las variables, con un pseudo R-cuadrado de 0.9152, indicando que explica aproximadamente el 91.52% de la variabilidad. El p-valor significativo (5.376e-136) sugiere que el modelo es preciso. De los 16 coeficientes de regresión, seis son significativos: texture_mean, concavity_mean, area_se, symmetry_se, fractal_dimension_se y symmetry_worst. Los coeficientes positivos (texture_mean, concavity_mean, area_se, symmetry_worst) aumentan la probabilidad de que el tumor sea maligno, mientras que los negativos (symmetry_se, fractal_dimension_se) la disminuyen.
En la matriz de confusión de los datos de entrenamiento, el modelo predijo correctamente el 98.24% de los casos, con un 1.76% de errores. En los datos de prueba, el modelo mantuvo una exactitud del 98.24%, reduciendo el número de falsos negativos de 7 a 5. Estos resultados indican que el modelo de regresión logística es altamente preciso y eficiente para la detección de cáncer de mama.
Inspiración y agradecimiento
Este proyecto se inspiró en este trabajo compartido en Kaggle Feature Selection and Data Visualization (kaggle.com), el cual ofreció valiosas percepciones sobre el aprendizaje. Agradezco enormemente al autor por compartir su conocimiento y recursos con la comunidad de código abierto.

## Estado del proyecto
Finalizado 
