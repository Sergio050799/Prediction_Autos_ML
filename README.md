### Precio Sobre Ruedas 🚘

### Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning para predecir el precio óptimo de un vehículo usado en función de sus características. Actualmente, el concesionario fija los precios de manera subjetiva, lo que genera inconsistencias y pérdidas de negocio. Con este modelo buscamos automatizar la tasación de vehículos, mejorar la precisión en la fijación de precios y aumentar la rentabilidad.

### Tecnologías Utilizadas

- **Python**
- **Pandas y NumPy**: para manipulación y análisis de datos.
- **Matplotlib y Seaborn**: para visualización de datos.
- **Scikit-learn y XGBoost**: para modelado y evaluación de algoritmos de ML.

### Análisis Exploratorio de Datos (EDA)

- **Limpieza y transformación de datos**: Tratamiento de nulos y duplicados.
- **Transformación logarítmica** para normalizar la variable objetivo.
- **Normalización** con PowerTransformer.
- **Visualización de relaciones entre variables**.
- **Codificación de variables categóricas** (Label Encoding & One Hot Encoding).

### Variables Clave

- Año de fabricación / antigüedad del vehículo.
- Kilometraje.
- Cilindrada (EngineLiters).
- Tipo de combustible (FuelType).
- Transmisión automática o manual.
- Cantidad de cilindros.

### Modelos Evaluados

Se evaluaron varios modelos con y sin reducción de dimensionalidad (PCA), y se aplicó optimización de hiperparámetros.

### Resultados Comparativos

| Modelo                       | Tipo      | MAE    | RMSE   | R²     |
|------------------------------|-----------|--------|--------|--------|
| XGBoost - Optimizado         | Sin PCA   | 0.1184 | 0.1661 | 0.9287 |
| XGBoost                       | Sin PCA   | 0.1206 | 0.1710 | 0.9245 |
| Random Forest - Optimizado   | Sin PCA   | 0.1285 | 0.1841 | 0.9124 |
| Random Forest                 | Sin PCA   | 0.1324 | 0.1866 | 0.9100 |
| Regresión Lineal              | Sin PCA   | 0.2179 | 0.2889 | 0.7844 |
| SVM - Optimizado             | Sin PCA   | 0.2118 | 0.2989 | 0.7692 |
| KNN - Optimizado             | Sin PCA   | 0.2851 | 0.3953 | 0.5963 |
| KNN                           | Sin PCA   | 0.3431 | 0.4708 | 0.4273 |
| SVM                           | Sin PCA   | 0.4224 | 0.5507 | 0.2164 |
| KNN                           | Con PCA   | 0.4333 | 0.5774 | 0.1386 |
| SVM                           | Con PCA   | 0.4727 | 0.6095 | 0.0401 |
| Regresión Lineal              | Con PCA   | 0.4756 | 0.6131 | 0.0287 |

### Métricas de Evaluación

- **MAE (Mean Absolute Error)**: Promedio de los errores absolutos. Cuanto más bajo, mejor.
- **RMSE (Root Mean Squared Error)**: Penaliza más los errores grandes.
- **R² (Coeficiente de Determinación)**: Mide qué tan bien el modelo explica la variabilidad del precio.

### Modelo Final Seleccionado

- **XGBoost Optimizado (sin PCA)**

| Métrica | Valor   |
|---------|---------|
| MAE     | 0.1184  |
| RMSE    | 0.1661  |
| R²      | 0.9287  |

Este modelo fue seleccionado por:

- Tener el mejor desempeño en todas las métricas.
- Gran capacidad de generalización.
- Buen equilibrio entre precisión y eficiencia computacional.

### Impacto Esperado en el Negocio

Con este modelo, el concesionario podrá:

- **Automatizar** la tasación de vehículos de forma precisa y consistente.
- **Mejorar la competitividad** al alinear los precios con el mercado.
- **Maximizar la rentabilidad** evitando la subvaloración o sobrevaloración.
- **Agilizar el proceso de ventas** al dar mayor confianza a clientes y vendedores.
- **Tomar decisiones basadas en datos reales**, no intuición.

### Futuras Mejoras

- Integración con dashboards de visualización (Power BI / Streamlit).
- Ajustes automáticos según tendencias del mercado.
- Entrenamiento periódico del modelo con nuevos datos.

### Proyecto desarrollado para mejorar la toma de decisiones en el sector automotriz mediante Machine Learning.
