#  Análisis Exploratorio y Modelado Predictivo de Precios de Viviendas

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning capaz de predecir el precio de venta de propiedades en India. El flujo de trabajo abarca desde la limpieza y exploración de datos hasta el entrenamiento y validación de los modelos predictivos.

## Objetivo
Predecir el precio de venta (en lacs) basándose en características como ubicación, metros cuadrados, estado de construcción y tipo de vendedor, para asistir en la tasación automática de inmuebles.

## Tecnologías Utilizadas
* **Python 3**
* **Pandas** 
* **NumPy**
* **Matplotlib & Seaborn:**
* **Scikit-Learn:** 

## Estructura del Proyecto

1.  **`EDA.ipynb` (Análisis Exploratorio de Datos):**
    * Limpieza de valores nulos y tratamiento de outliers usando Rango Intercuartílico (IQR).
    * Análisis univariado y bivariado de las características.
    * Estudio de correlaciones para selección de variables.
    * Transformación de variables categóricas.

2.  **`modelos.ipynb` (Modelado Predictivo):**
    * Ingeniería de características (Feature Engineering) y escalado de datos (StandardScaler).
    * Entrenamiento de múltiples modelos: Regresión Lineal, Ridge, Lasso, KNN, Decision Tree y Bagging Regressor.
    * Evaluación de métricas: RMSE, MAE y R².
    * Optimización de hiperparámetros.

## 📊 Resultados Destacados
* El modelo de **Bagging Regressor** obtuvo el mejor desempeño con un **R² de 0.82**.
* Se identificó que aplicar una transformación logarítmica al precio objetivo mejoró significativamente la homocedasticidad de los residuos.
* Se detectó una menor precisión en propiedades de muy alto valor (lujo), lo cual se documenta como una oportunidad de mejora futura.

## 🚀 Cómo ejecutar este proyecto

1.  Clonar el repositorio.
2.  Instalar las dependencias:
    pip install -r requirements.txt
3.  Abrir los notebooks en orden: primero `EDA.ipynb` y luego `modelos.ipynb`.