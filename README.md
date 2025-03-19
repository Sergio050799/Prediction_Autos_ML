# Precio Sobre Ruedas 🚘

## Descripción del Proyecto
Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning para predecir el precio óptimo de un vehículo usado en función de sus características. Actualmente, el concesionario fija los precios de manera subjetiva, lo que genera inconsistencias y pérdidas de negocio. Con este modelo, buscamos automatizar la tasación de vehículos y mejorar la rentabilidad.

---

## Tecnologías Utilizadas

- **Python** 
- **Pandas y NumPy**: Para manipulación de datos.
- **Matplotlib y Seaborn**: Para visualización .
- **Scikit-learn y XGBoost**: Para modelado de Machine Learning.

---

## Análisis Exploratorio de Datos (EDA)
- Se realizó un análisis detallado de los datos para entender la distribución de precios, detectar outliers y evaluar la relación entre variables.
- Se identificaron variables clave como:
  - Año del vehículo.
  - Kilometraje.
  - Tipo de motor.
  - Consumo de combustible.
- Tratamiento de valores faltantes y datos inconsistentes mediante limpieza y transformación de datos.

---

## Modelos Evaluados

Se probaron tres modelos de Machine Learning para la predicción de precios:

| Modelo            | MSE    | R² Score |
|--------------------|--------|----------|
| XGBoost           | 0.0343 | 0.9137   |
| Random Forest      | 0.0396 | 0.9004   |
| Regresión Lineal   | 0.0775 | 0.8050   |

El modelo **XGBoost** mostró el mejor rendimiento en términos de precisión y generalización, por lo que fue seleccionado como modelo final:

- **Menor MSE (0.0343)**: Predicciones más precisas.
- **Mayor R² (0.9137)**: Explica el 91.37% de la variabilidad en los precios de los vehículos.
- **Balance entre sesgo y varianza**, evitando el sobreajuste.
- **Eficiencia computacional**, superando a modelos como Random Forest.

---

## Impacto Esperado
Este modelo permitirá al concesionario:
- Automatizar la tasación de vehículos, eliminando la subjetividad en la fijación de precios.
- Mejorar la competitividad mediante precios más precisos y alineados con el mercado.
- Maximizar la rentabilidad al evitar la subvaloración o sobrevaloración de los autos.
- Agilizar el proceso de ventas, generando confianza en clientes y vendedores mediante decisiones respaldadas por datos.

---
