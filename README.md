# 📊 Telecom X: Analisis y Predicción de Fuga de Clientes (Churn)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## 🎯 Objetivo del Proyecto
Este proyecto aborda el desafío del **Churn (cancelación de clientes)** en la empresa Telecom X desde dos frentes: un análisis exploratorio profundo (EDA) para entender el pasado, y el entrenamiento de modelos de **Machine Learning** para predecir el futuro y proponer estrategias de retención.

## 🚀 Fases del Proyecto

### Fase 1: Analisis Exploratorio y ETL
* **Limpieza y Normalización:** Extracción de datos desde JSON, aplanado de estructuras anidadas y tratamiento de valores nulos/duplicados.
* **Feature Engineering:** Creación de nuevas métricas financieras como `Cuentas_Diarias`.
* **EDA:** Identificación visual de patrones de fuga mediante Seaborn y Matplotlib.

### Fase 2: Modelado Predictivo (Machine Learning)
* **Preprocesamiento:** Aplicación de **One-Hot Encoding** para la conversión de variables categóricas y **StandardScaler** para la normalización de escalas.
* **Balanceo de Datos:** Implementación de **SMOTE** para corregir el desbalance de clases y evitar sesgos en el entrenamiento.
* **Entrenamiento y Evaluación:** Comparación de algoritmos (**Regresión Logística** vs. **Random Forest**). Evaluación exhaustiva utilizando Matrices de Confusión, Exactitud (Accuracy) y Sensibilidad (Recall). 
* **Optimización:** Detección de *overfitting* en Random Forest y ajuste mediante afinación de hiperparámetros (poda del árbol).

## 📈 Conclusiones y Explicabilidad del Modelo
A través del análisis de *Feature Importance* e inspección de coeficientes, el modelo determinó que los factores críticos de fuga son:
1. **Tipo de Contrato:** Los esquemas "Month-to-month" presentan el mayor riesgo.
2. **Antigüedad (Tenure):** Los primeros meses son críticos; a mayor antigüedad, la probabilidad de fuga cae drásticamente.
3. **Facturación:** Cargos recurrentes altos sin una propuesta de valor clara impulsan las bajas.

## 🛠️ Tecnologías y Librerías Utilizadas
* `pandas`, `numpy` (Manipulación de datos)
* `matplotlib`, `seaborn` (Visualización)
* `scikit-learn`, `imblearn` (Machine Learning y Balanceo)

---
✍️ **Autor:** Adriel Barrios
🎓 **Contexto:** Challenge Data Science - Alura LATAM
