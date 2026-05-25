# Proyecto IA
# Proyecto: Agente de IA con Mistral

## Bitácora de cambios
- **Commit [25/05]:** Normalización del dataset `sales_data_sample.csv`.
    - Se eliminaron valores nulos en columnas geográficas y se reemplazaron por 'N/A'.
    - Se estandarizó el formato de la columna `ORDERDATE` a datetime.
    - Se generó el archivo `ventas.csv` como base de conocimiento limpia para el modelo.
