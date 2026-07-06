# Dataset

Este directorio contiene el dataset utilizado en el proyecto.

## Archivos

- `processed/fire_summary_refined_2024.csv`: tabla principal de eventos de fuego refinados.
- `geo/fire_perimeters_refined_2024.gpkg`: geometrías de perímetros refinados.

## Fuente primaria

Las detecciones activas de fuego utilizadas como insumo provienen de sensores satelitales VIIRS/FIRMS.

## Producto procesado

Los eventos y perímetros fueron generados mediante una cadena PyroTrack FEDS-like, que consolida detecciones activas en objetos de fuego mediante agrupamiento espacio-temporal, tracking y generación de perímetros.
