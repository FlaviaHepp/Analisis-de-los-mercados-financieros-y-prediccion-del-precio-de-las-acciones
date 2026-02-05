# 📈Análisis de los mercados financieros y predicción del precio de las acciones

## 📌Descripción del proyecto

Este proyecto realiza un análisis exploratorio y predictivo de datos financieros, integrando información histórica de acciones del NASDAQ, tipos de cambio y criptomonedas desde el año 2003 hasta 2023.

El trabajo combina visualización financiera, análisis estadístico y machine learning para estudiar el comportamiento de los precios y construir un modelo de predicción del precio de cierre de acciones.

## 🎯Objetivos

- Analizar la evolución histórica de activos financieros
- Explorar volatilidad, retornos y tendencias
- Visualizar precios mediante gráficos de series temporales y velas
- Reducir dimensionalidad con PCA
- Crear variables temporales (lags)
- Entrenar un modelo de regresión para predecir precios de cierre

## 📂Conjunto de datos

- Los datasets incluyen datos financieros de:
  - Acciones (NASDAQ): AAPL, AMD, entre otras
  - Criptomonedas
  - Mercado de divisas (Forex)
  - Variables principales
  - Open – Precio de apertura
  - High – Precio máximo
  - Low – Precio mínimo
  - Close – Precio de cierre
  - Volume – Volumen negociado
  - Year
  - YTD Gain – Ganancia acumulada del año
  - Período cubierto: 01/01/2003 – 11/06/2023

## 🛠️Tecnologías utilizadas

- Python
- Pandas / NumPy – Manipulación de datos
- Matplotlib / Seaborn – Visualización
- Plotly – Gráficos interactivos (candlestick)
- Scikit-learn – PCA, división de datos
- CatBoost – Modelo de regresión
- TQDM – Seguimiento de procesos

## 🔍Metodología

1️⃣ Análisis Exploratorio (EDA)
- Inspección del dataset
- Estadísticas descriptivas
- Visualización de precios de cierre
- Análisis de retornos diarios
- Medias móviles y desviación estándar
- Histogramas de retornos
- Matriz de correlación implícita

2️⃣ Visualización financiera
- Series temporales de precios
- Gráficos de velas (Candlestick)
- Análisis de volatilidad

3️⃣ Feature Engineering
- Selección de variables OHLCV
- Reducción de dimensionalidad con PCA
- Creación de:
  - Lags diarios (1 a 6 días)
  - Lags semanales (1 a 3 semanas)

4️⃣ Modelado predictivo
- División de datos en entrenamiento y test
- Entrenamiento con CatBoostRegressor
- Evaluación del modelo con MAE (Mean Absolute Error)

## 📊Resultados

- El modelo logra predecir el precio de cierre con un error absoluto medio (MAE) competitivo
- PCA permite reducir ruido y dimensionalidad sin perder información relevante
- Las variables temporales capturan dependencia histórica de los precios


## 🚀Posibles mejoras futuras

- Implementar modelos de series temporales (ARIMA, LSTM)
- Comparar distintos algoritmos de regresión
- Optimizar hiperparámetros
- Incorporar análisis multiactivo
- Crear un dashboard interactivo
