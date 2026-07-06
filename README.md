# Perfilado no supervisado de eventos de fuego en Paraguay durante 2024

Este proyecto aplica técnicas de aprendizaje no supervisado para identificar perfiles de eventos de fuego en Paraguay durante 2024, utilizando productos PyroTrack FEDS-like derivados de detecciones satelitales VIIRS/FIRMS.

## Objetivo

Identificar grupos de eventos de fuego con características similares a partir de atributos espaciales, temporales, geométricos y de intensidad.

## Dataset

El dataset principal se encuentra en:

- `data/processed/fire_summary_refined_2024.csv`
- `data/geo/fire_perimeters_refined_2024.gpkg`

El producto contiene objetos de fuego refinados generados mediante una cadena PyroTrack FEDS-like, basada en detecciones activas satelitales, agrupamiento espacio-temporal, seguimiento de eventos y generación de perímetros.

## Metodología prevista

1. Análisis exploratorio de datos.
2. Limpieza y selección de variables.
3. Escalado de variables numéricas.
4. Aplicación de modelos de clustering.
5. Evaluación mediante métricas internas.
6. Visualización e interpretación de perfiles.

## Modelos

Se evaluarán al menos dos algoritmos de clustering:

- HDBSCAN o DBSCAN.
- Agglomerative Clustering o Gaussian Mixture Model.

K-Means podrá utilizarse únicamente como referencia.

## Métricas

- Silhouette Score.
- Davies-Bouldin Index.
- Calinski-Harabasz Index.

## Visualizaciones previstas

- Serie mensual de actividad de fuego.
- Mapa de eventos/perímetros.
- Proyección UMAP de los eventos.
- Comparación de métricas entre modelos.
- Perfil de variables por cluster.

## Autores

Diego Baez
