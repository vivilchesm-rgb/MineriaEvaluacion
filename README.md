# 🎬 Minería de Datos: Análisis de Rentabilidad y Éxito en el Cine (Blockbusters)

## 📋 Información del Proyecto
*   **Integrantes:** [Tu Nombre] - [Nombre de tu Compañero]
*   **Docente:** Carlos Muñoz
*   **Dataset:** [Blockbuster Cinematic Archive (expensive_movie.csv)](https://www.kaggle.com/datasets/jaydeepahir18/hollywoods-most-expensive-blockbusters)

## 📝 Descripción
Este proyecto realiza un **Análisis Exploratorio de Datos (EDA)** exhaustivo sobre un conjunto de datos de producciones cinematográficas de alto presupuesto extraído de Kaggle. El objetivo es identificar patrones económicos (inversión vs. recaudación) y factores sociales (popularidad, idiomas y géneros) que determinan el éxito comercial en la industria. El análisis incluye técnicas avanzadas de preparación de datos para futuros modelos de **Machine Learning**.

## 🚀 Fases del Proyecto

### 1. Importación y Configuración
*   Configuración del entorno en **Google Colab** y carga de librerías base: `Pandas`, `NumPy`, `Matplotlib` y `Seaborn`.
*   Carga del dataset `expensive_movie.csv` y validación de sus dimensiones iniciales.

### 2. Entendimiento y Mapeo de Datos (Data Dictionary)
*   **Mapeo de Variables:** Creación de un diccionario para estandarizar el conocimiento sobre columnas como `Budget`, `Revenue`, `Popularity` y `Genres`.
*   **Inspección de Tipos:** Aseguramos que las variables numéricas y categóricas tengan el formato adecuado para el procesamiento en Python.

### 3. Limpieza y Curación de Datos
*   **Tratamiento de Valores en Cero:** Filtrado de registros con presupuesto o ingresos en 0 para eliminar datos incompletos que sesgan el análisis de rentabilidad.
*   **Manejo de Nulos:** Confirmación de integridad del dataset y eliminación de registros inválidos.

### 4. Ingeniería de Variables (Profit Analysis)
*   **Cálculo de Profit:** Creación de la variable `Profit` (Ganancia Neta) restando el `Budget` al `Revenue`.
*   **Detección de Extremos:** Identificación de los 10 mayores éxitos comerciales y los fracasos financieros más notables de la historia.

### 5. Análisis Exploratorio de Datos (EDA)
*   **Evolución Temporal:** Análisis del crecimiento del presupuesto promedio por año y su relación con la recaudación según la época.
*   **Análisis Social:** Cruzamiento de la métrica de `Popularity` con la calificación promedio (`Vote_Average`) para entender el comportamiento de la audiencia.
*   **JointPlot de Densidad:** Uso de visualizaciones avanzadas para observar la concentración de producciones según sus niveles de inversión.

### 6. Transformación para Algoritmos (Encoding)
*   **One-Hot Encoding:** Aplicación de la técnica en la columna `Status` para evitar órdenes de importancia inexistentes en las categorías cualitativas.
*   **Label Encoding:** Codificación numérica de idiomas originales para permitir su procesamiento en modelos estadísticos y cálculos de **Ganancia de Información**.

### 7. Importancia de Variables y Correlación
*   **Matriz de Correlación:** Uso de Heatmaps para cuantificar la fuerza de la relación entre variables financieras.
*   **Feature Importance:** Implementación de un modelo base de **Random Forest** para determinar qué variables (como el `Budget` o el `Vote_Count`) influyen más en la predicción del éxito financiero.

## 🛠️ Tecnologías Utilizadas
*   **Python:** Lenguaje principal.
*   **Pandas & NumPy:** Manipulación y limpieza de estructuras de datos.
*   **Seaborn & Matplotlib:** Visualización de datos y gráficos estadísticos.
*   **Scikit-learn:** Preparación de datos y modelos de importancia de variables.
