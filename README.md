# Sistema de Agentes de IA - Predicción y Consulta de Transfermarkt

Este proyecto implementa un pipeline completo de Inteligencia Artificial compuesto por tres agentes especializados para procesar datos de futbolistas, entrenar modelos predictivos de valor de mercado y ofrecer una interfaz de consulta generativa.

## Estructura del Sistema

El proyecto está dividido en 3 agentes autónomos dentro de `football_players.py`:

1. **Agente 1 (Normalizador):** Se encarga de la carga del dataset (`players.csv`), la limpieza de datos, la imputación de valores nulos (usando medianas y categorías por defecto), el escalado con `StandardScaler` y la codificación One-Hot para exportar un archivo limpio (`players_clean.csv`).
2. **Agente 2 (Entrenador):** Divide los datos en conjuntos de entrenamiento y prueba, entrena modelos de Regresión Lineal y Random Forest, evalúa las métricas ($R^2$ y MAE) y exporta un informe con el modelo ganador en `resultados_entrenamiento.json`.
3. **Agente 3 (Comunicador):** Consolida la memoria de los agentes previos e inicia una interfaz interactiva en la consola que se conecta con la API de **Gemini 2.5 Flash** para responder preguntas del usuario de forma profesional y contextualizada.

## Requisitos e Instalación

Para ejecutar este proyecto, necesitas instalar las siguientes librerías de Python:

```bash
pip install pandas numpy scikit-learn requests
