# Proyecto IA
# Proyecto: Agente de IA con Mistral

## Bitácora de cambios
- **Commit [25/05]:** Normalización del dataset `sales_data_sample.csv`.
    - Se eliminaron valores nulos en columnas geográficas y se reemplazaron por 'N/A'.
    - Se estandarizó el formato de la columna `ORDERDATE` a datetime.
    - Se generó el archivo `ventas.csv` como base de conocimiento limpia para el modelo.
    
- Commit [25/05]: Implementación de Agente Inteligente con Mistral Small y LangChain.
    - Se configuró el pandas_dataframe_agent con tool-calling para interacción precisa.
    - Se definió un prefix_prompt con contexto de negocio para asegurar la integridad matemática en las consultas.
    - Se añadieron pruebas automatizadas para verificar el razonamiento lógico del modelo sobre el dataset.

- Commit [25/05]: Implementación de Agente Inteligente con Mistral Small y LangChain.
    - Se configuró el pandas_dataframe_agent con tool-calling para consultas precisas sobre el corpus.
    - Se integró un prefix_prompt con contexto de negocio para asegurar resultados matemáticos exactos.
    - Se desarrollaron pruebas automatizadas de razonamiento lógico sobre el dataset ventas.csv.
