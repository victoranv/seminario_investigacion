# Detección y Prevención de Actividades Delictivas en Bucaramanga

Este proyecto tiene como objetivo la detección y prevención de actividades delictivas en la ciudad de Bucaramanga utilizando técnicas de machine learning, particularmente un modelo de **clustering** para identificar las zonas de mayor ocurrencia de delitos y un análisis de series de tiempo para predecir futuros delitos.

## Descripción del Proyecto

El proyecto se centra en analizar datos de delitos en Bucaramanga, específicamente en el tipo de delito de **hurto a personas**. Los datos utilizados fueron proporcionados por el sistema de información del municipio y contienen información detallada sobre la ubicación de los delitos, la hora de ocurrencia, el tipo de delito, el barrio, entre otros.

Utilizando el algoritmo de **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise), el modelo busca identificar patrones y zonas de alta densidad de delitos. Posteriormente, se generaron visualizaciones interactivas en Power BI y mapas interactivos con **Folium** para mostrar las áreas con mayor riesgo.

## Metodología

### 1. **Preprocesamiento de los Datos**
   - Se limpiaron los datos eliminando valores nulos y registros irrelevantes.
   - Se normalizaron las variables numéricas, como las coordenadas de latitud y longitud, para facilitar la identificación de patrones.

### 2. **Modelo de Clustering: DBSCAN**
   - **DBSCAN** fue utilizado para encontrar clusters de delitos basados en la proximidad geográfica y la hora de ocurrencia.
   - Los clusters fueron analizados para identificar las zonas con mayor densidad de delitos.
   - El modelo también identificó puntos de "ruido" (delitos fuera de los patrones comunes).

### 3. **Visualización de los Resultados**
   - Se creó un mapa interactivo utilizando **Folium** para visualizar los clusters de delitos en Bucaramanga.
   - Los diferentes clusters se representaron con colores específicos para facilitar su interpretación.

### 4. **Predicción de Delitos**
   - Se desarrolló un modelo de series de tiempo para predecir la frecuencia de delitos en 2025, basándose en los datos históricos.

## Resultados

El modelo de clustering identificó múltiples zonas en Bucaramanga con alta concentración de delitos. A través de la visualización interactiva, se pudo identificar claramente las áreas más peligrosas para la intervención preventiva.

Se utilizó un mapa de calor en **Power BI** para mostrar las zonas con más actividad delictiva, proporcionando información útil para la toma de decisiones y la asignación de recursos.

### Visualización de Clusters
El enlace a la visualización interactiva de los clusters es el siguiente:
[Ver Mapa de Clusters en Power BI](https://app.powerbi.com/view?r=eyJrIjoiNGI4ZTI0NjktNGRlZC00N2FkLTg3M2UtZDEyNWYzNDEwNWU3IiwidCI6Ijg3NDg5NWUwLWQwYjYtNDkzZC05N2YxLWE1MzMxODc0M2I3ZSIsImMiOjR9)

### Mapa de Clusters de Bucaramanga (Generado con Folium)
El mapa interactivo con los clusters generados puede visualizarse a través del siguiente enlace:
[Ver Mapa Interactivo de Clusters](ruta/del/archivo/prueba_clust.html)

## Instalación y Uso

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/usuario/detecion-actividades-delictivas.git
   cd deteccion-actividades-delictivas
    ```   

2. **Ejecutar el script Modelo clustering:**
   ```bash
    Modelo clustering.ipynb
    ```
