# **📊 Predicción de Precios de Viviendas en California con Machine Learning**


**Sarahi Lilian Tello Torres**
**[Data Scientist | Machine Learning & Applied Mathematics]**

📍 *Ciudad de México, México*
🔗 [GitHub](https://github.com/Sarahitello) | [LinkedIn](https://www.linkedin.com/in/sarahi-lilian-tello-torres-568741202)

---
## 📌 Descripción
Este proyecto aplica **técnicas avanzadas de Machine Learning** para predecir el valor medio de las viviendas en **California**, utilizando el dataset oficial de **scikit-learn**. Se emplean modelos de **ensamble** como **Random Forest** y **Gradient Boosting**, que permiten capturar relaciones no lineales y manejar valores atípicos de manera robusta.

**Aplicaciones prácticas:**
- **Análisis inmobiliario**: Predicción de precios para inversiones y valoración de propiedades.
- **Toma de decisiones**: Soporte para políticas públicas y desarrollo urbano.
- **Data Science**: Ejemplo práctico de modelado predictivo con datos reales.

---

## 🔧 Tecnologías Utilizadas
| Tecnología       | Descripción                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Python**       | Lenguaje principal para análisis y modelado.                              |
| **Pandas**       | Manipulación y análisis de datos.                                          |
| **NumPy**        | Cálculos numéricos y operaciones con arrays.                             |
| **Scikit-learn** | Librería para Machine Learning (Random Forest, Gradient Boosting).         |
| **Matplotlib**   | Visualización de datos y resultados.                                      |
| **Seaborn**      | Gráficos estadísticos avanzados.                                           |
| **Google Colab** | Entorno de ejecución en la nube con soporte para análisis de datos.     |

---

## 🚀 ¿Cómo Ejecutar el Proyecto?
1. **Abrir en Google Colab**:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sarahitello/Proyecto-IA-Vision-Computacional/blob/main/Sistema_de_detección_automática_de_objetos_en_imágenes.ipynb)

3. **Instalar dependencias** (si es necesario):
   ```bash
   !pip install pandas numpy scikit-learn matplotlib seaborn
   ```

4. **Cargar el dataset**:
   ```python
   from sklearn.datasets import fetch_california_housing
   df = fetch_california_housing(as_frame=True).frame
   ```

5. **Ejecutar el notebook** para ver el análisis exploratorio, limpieza de datos, modelado y evaluación.

---

## ✨ Funcionalidades
1. **Análisis Exploratorio de Datos (EDA)**:
   - Visualización de distribuciones y correlaciones entre variables.
   - Identificación de valores atípicos y patrones espaciales.

2. **Limpieza de Datos**:
   - Imputación de valores faltantes con la mediana.
   - Eliminación de outliers usando el método **IQR**.

3. **Modelado Predictivo**:
   - **Random Forest**: Modelo robusto para capturar relaciones no lineales.
   - **Gradient Boosting**: Modelo secuencial para corregir errores y mejorar precisión.

4. **Evaluación de Modelos**:
   - Métricas de desempeño: **MAE, RMSE, R²**.
   - Análisis de residuales para validar ajustes.

5. **Interpretabilidad**:
   - Gráficos de importancia de variables para entender el impacto de cada feature.

---

## 📊 Dataset
- **Nombre del Dataset**: **California Housing Dataset** (scikit-learn).
- **Descripción**: Conjunto de datos con variables geográficas y demográficas de viviendas en California, incluyendo:
  - `longitude` y `latitude`: Coordenadas geográficas.
  - `housingMedianAge`: Edad media de las viviendas.
  - `totalRooms` y `totalBedrooms`: Número total de habitaciones y dormitorios.
  - `population`: Población del área.
  - `MedHouseVal`: Valor medio de la vivienda (variable objetivo).
- **Fuente**: [scikit-learn Datasets](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset).

---

## 🤖 Modelo
- **Modelos Utilizados**:
  - **Random Forest Regressor**:
    - `n_estimators=300`, `random_state=42`.
    - **Métricas**: MAE = 29,670 | RMSE = 44,970 | R² = 0.78.
  - **Gradient Boosting Regressor**:
    - `n_estimators=300`, `learning_rate=0.05`, `max_depth=3`.
    - **Métricas**: MAE = 36,386 | RMSE = 51,364 | R² = 0.71.

- **Conclusiones**:
  - **Random Forest** ofrece mayor estabilidad e interpretabilidad.
  - **Gradient Boosting** logra menor error predictivo en algunos casos.
  - La **ubicación geográfica** es el principal determinante del valor de la vivienda.
