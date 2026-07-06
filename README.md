# PyroTrack Clustering Paraguay 2024

Proyecto final de aprendizaje no supervisado aplicado al perfilado de eventos de fuego en Paraguay durante 2024.

El objetivo es identificar perfiles de eventos de fuego mediante clustering, usando atributos espaciales, temporales, geométricos y de intensidad derivados de productos PyroTrack FEDS-like.

## Dataset

El dataset principal corresponde a eventos de fuego refinados para Paraguay en 2024:

- `data/processed/fire_summary_refined_2024.csv`
- `data/geo/fire_perimeters_refined_2024.gpkg`

El producto fue generado a partir de detecciones activas VIIRS/FIRMS mediante una cadena PyroTrack FEDS-like, que agrupa detecciones espacio-temporales, realiza seguimiento de objetos de fuego y genera perímetros mediante geometrías tipo alpha-shape.

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

K-Means podrá utilizarse como referencia, pero no como uno de los dos modelos principales.

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

## Estructura


data/
  processed/
  geo/
notebooks/
results/
  figures/
docs/

Autor
Diego Baez
