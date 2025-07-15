# Recomendación de Vinos con KNN, PCA y Análisis Exploratorio

Este repositorio presenta una solución basada en aprendizaje no supervisado para encontrar los vinos más similares a una referencia dada, utilizando el algoritmo KNN, reducción de dimensionalidad con PCA y visualización 2D.

## Objetivo

Identificar los 5 vinos más similares a un vino de referencia según sus características químicas, y estimar el contenido promedio de alcohol entre ellos.

## Metodología

### 1. Carga y preparación de datos
- Lectura del archivo `wine-clustering.csv` con `pandas`
- Estandarización de variables con `StandardScaler`
- Definición de un vino de referencia con 13 características

### 2. Reducción de dimensionalidad
- Aplicación de `PCA` para visualizar los datos en 2D
- Transformación de los vinos y del vino de referencia en el espacio PCA

### 3. Algoritmo KNN
- Uso de `NearestNeighbors` con métrica euclidiana y `n_neighbors=5`
- Identificación de los 5 vinos más cercanos al de referencia
- Cálculo del promedio de alcohol de los vecinos

### 4. Visualización
- Gráfico en 2D de los vinos en el plano PCA
- Conectores entre el vino de referencia y sus vecinos más cercanos
- Etiquetado claro para interpretación visual

### 5. Resumen numérico
- Impresión de características de los vinos similares
- Listado de valores individuales de alcohol
- Estimación promedio para el vino de referencia

## Tecnologías utilizadas

- Python 3.x  
- pandas  
- numpy  
- scikit-learn  
- matplotlib

## Conclusiones

- Los vecinos más cercanos comparten valores similares en alcohol, color, fenoles y flavonoides.
- PCA facilita la visualización interpretativa en dos dimensiones.
- KNN se muestra eficaz para recomendar vinos según perfil químico.
