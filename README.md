
# Análisis y predicción del desempleo en Costa Rica

## Descripción
Este proyecto analiza la relación entre desempleo, inflación y crecimiento del PIB en Costa Rica. Primero se desarrolla un análisis econométrico con regresión lineal múltiple y posteriormente se compara el desempeño predictivo de distintos modelos de Machine Learning, incluyendo regresión lineal con rezagos y Random Forest.

## Objetivo
Explorar la relación entre variables macroeconómicas clave y evaluar qué modelo ofrece la mejor capacidad predictiva para el desempleo en Costa Rica.

## Fuente de datos
Los datos fueron obtenidos mediante la API del Banco Mundial para Costa Rica.

Variables utilizadas:
- Desempleo total (% de la fuerza laboral)
- Inflación, precios al consumidor (anual %)
- Crecimiento del PIB (anual %)

## Metodología
1. Extracción de datos desde la API del Banco Mundial.
2. Construcción y limpieza de los dataframes.
3. Análisis descriptivo y matriz de correlación.
4. Estimación de un modelo de regresión econométrica OLS.
5. Construcción de modelos predictivos con validación temporal.
6. Comparación de:
   - modelo base,
   - modelo con `lag1`,
   - modelo con `lag1 + lag2`,
   - Random Forest.

## ## Tecnologías utilizadas
## Tecnologías utilizadas
- Python
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- scikit-learn
- requests
- Jupyter Notebook
- APIs REST del Banco Mundial

## Resultados principales
- La regresión OLS mostró relaciones significativas entre las variables macroeconómicas y el desempleo.
- El modelo con `lag1` fue el mejor modelo predictivo.
- La incorporación de `lag2` no mejoró el desempeño.
- Random Forest no superó al modelo lineal con rezago.

## Conclusión
El proyecto muestra que, para este conjunto de datos y tamaño de muestra, un modelo lineal con componente temporal captura mejor la dinámica del desempleo que un modelo más complejo como Random Forest.

## Limitaciones
- Tamaño de muestra reducido.
- Pocas variables explicativas.
- Posible presencia de autocorrelación.
- Los modelos podrían mejorar con más información macroeconómica.

## Posibles extensiones
- Walk-forward validation.
- ARIMA / SARIMA / ARIMAX.
- Nuevas variables macroeconómicas.
- Modelos de boosting como XGBoost.

## Estructura del repositorio
- `data/`: archivos de datos.
- `notebooks/`: notebooks de análisis y modelado.
- `outputs/`: gráficos, tablas e informes exportados.
- `README.md`: descripción general del proyecto.
- `requirements.txt`: dependencias del proyecto.

## Project Information

- Version: 1.0

- Status: Production Release

- Release Date: July 2026

- Country: Costa Rica

- Type: Portfolio Project

- Language: Python

---

This project represents the first professional data analytics project developed as part of my portfolio.
