# ml-project-zyra


## English

**Project:** Data Analysis and Predictive Modeling for Zyra Company

### Context
Zyra is an industrial company focused on the extraction and purification of gold. The company collects large amounts of process data from various stages of its production line. The main objective of this project is to analyze this data and develop a predictive model to estimate gold recovery rates at different purification stages, helping Zyra optimize its processes and improve efficiency.

### Methodology
The project follows a structured data science workflow:

1. **Data Collection and Understanding**
	- Datasets from Zyra's production process were provided, including full, training, and test sets.
	- Initial exploration identified missing values, outliers, and the structure of the data.

2. **Data Cleaning and Preprocessing**
	- Missing values were handled by replacing them with sentinel values (-1 or 1) depending on the column type.
	- Outliers and anomalies (e.g., near-zero concentrations) were detected and removed to ensure data quality.
	- Columns were reorganized for clarity and consistency across datasets.

3. **Exploratory Data Analysis (EDA)**
	- Visualizations and statistical analysis were performed to understand the distribution of key variables, such as metal concentrations and particle sizes.
	- Comparisons between training and test sets ensured that the model would generalize well.

4. **Feature Engineering**
	- New features were created, such as total concentrations of metals at different stages.
	- Only relevant features were selected for modeling, based on domain knowledge and data availability.

5. **Model Development**
	- Several regression models were trained: Linear Regression, Decision Tree, and Random Forest.
	- Model performance was evaluated using the sMAPE metric, which is robust to scale and interpretable for business stakeholders.
	- Cross-validation was used to select the best model and avoid overfitting.

6. **Model Evaluation and Interpretation**
	- The Decision Tree Regressor was selected as the best model, achieving a final sMAPE of ~7.83% in cross-validation and 10.15% on the test set.
	- The model's predictions were analyzed to ensure they made sense in the context of Zyra's operations.

### Results and Conclusions
- The Decision Tree model provides a reliable and interpretable solution for predicting gold recovery.
- The difference between cross-validation and test performance suggests some variability in the data, but the model remains robust.
- The project demonstrates the value of data-driven decision-making in industrial settings.

### Possible Improvements
- Incorporate more advanced models (e.g., Gradient Boosting, Neural Networks) for potentially better accuracy.
- Use domain-specific feature engineering to capture more process nuances.
- Deploy the model in a real-time monitoring system for continuous process optimization.

### Technologies Used
- Python, pandas, numpy, matplotlib, plotly, scikit-learn, scipy

---

---


## Español

**Proyecto:** Análisis de Datos y Creación de un Modelo Predictivo para la Empresa Zyra

### Contexto
Zyra es una empresa industrial dedicada a la extracción y purificación de oro. La compañía recopila grandes volúmenes de datos de sus procesos productivos. El objetivo principal de este proyecto es analizar estos datos y desarrollar un modelo predictivo para estimar la tasa de recuperación de oro en diferentes etapas de purificación, ayudando a Zyra a optimizar sus procesos y mejorar la eficiencia.

### Metodología
El proyecto sigue un flujo de trabajo estructurado de ciencia de datos:

1. **Recolección y Comprensión de Datos**
	- Se proporcionaron datasets del proceso productivo de Zyra: conjunto completo, entrenamiento y prueba.
	- La exploración inicial identificó valores nulos, atípicos y la estructura de los datos.

2. **Limpieza y Preprocesamiento de Datos**
	- Los valores nulos se trataron reemplazándolos por valores centinela (-1 o 1) según el tipo de columna.
	- Se detectaron y eliminaron valores atípicos y anomalías (por ejemplo, concentraciones cercanas a cero) para asegurar la calidad de los datos.
	- Las columnas se reorganizaron para mayor claridad y consistencia entre los datasets.

3. **Análisis Exploratorio de Datos (EDA)**
	- Se realizaron visualizaciones y análisis estadísticos para comprender la distribución de variables clave, como concentraciones de metales y tamaños de partículas.
	- Se compararon los conjuntos de entrenamiento y prueba para asegurar la capacidad de generalización del modelo.

4. **Ingeniería de Características**
	- Se crearon nuevas características, como concentraciones totales de metales en diferentes etapas.
	- Se seleccionaron solo las características relevantes para el modelado, basándose en conocimiento del dominio y disponibilidad de datos.

5. **Desarrollo del Modelo**
	- Se entrenaron varios modelos de regresión: Regresión Lineal, Árbol de Decisión y Random Forest.
	- El desempeño de los modelos se evaluó usando la métrica sMAPE, robusta y fácil de interpretar para el negocio.
	- Se utilizó validación cruzada para seleccionar el mejor modelo y evitar sobreajuste.

6. **Evaluación e Interpretación del Modelo**
	- El Árbol de Decisión fue seleccionado como el mejor modelo, logrando un sMAPE final de ~7.83% en validación cruzada y 10.15% en el set de prueba.
	- Se analizaron las predicciones del modelo para asegurar su coherencia con las operaciones de Zyra.

### Resultados y Conclusiones
- El modelo de Árbol de Decisión proporciona una solución confiable e interpretable para predecir la recuperación de oro.
- La diferencia entre el desempeño en validación cruzada y prueba sugiere cierta variabilidad en los datos, pero el modelo es robusto.
- El proyecto demuestra el valor de la toma de decisiones basada en datos en entornos industriales.

### Posibles Mejoras
- Incorporar modelos más avanzados (por ejemplo, Gradient Boosting, Redes Neuronales) para mejorar la precisión.
- Usar ingeniería de características específica del dominio para capturar más matices del proceso.
- Desplegar el modelo en un sistema de monitoreo en tiempo real para optimización continua del proceso.

### Tecnologías Utilizadas
- Python, pandas, numpy, matplotlib, plotly, scikit-learn, scipy