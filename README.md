# Predicción de Churn en Clientes de Telecomunicaciones

📌 **Descripción**

En esta segunda parte del proyecto se desarrollan modelos de **Machine Learning** para predecir la cancelación de clientes (**Churn**) en una empresa de telecomunicaciones.  
Se trabajó en Google Colab con Python, siguiendo fases estructuradas que incluyen balanceo de clases, entrenamiento de modelos, evaluación de métricas y análisis interpretativo de resultados.

---

## 🛠 Proceso realizado

1. **Preprocesamiento de datos**  
   - Imputación de valores nulos.  
   - Codificación de variables categóricas (One-Hot Encoding).  
   - Escalado de variables numéricas.  
   - Balanceo de clases con **SMOTE** (exploratorio, no aplicado al pipeline final).  

2. **Modelado predictivo**  
   - Entrenamiento de modelos base:  
     - **Regresión Logística**  
     - **Random Forest**  
   - Evaluación comparativa con métricas: Accuracy, Precision, Recall, F1-score y Matriz de Confusión.  

3. **Interpretación de modelos**  
   - Importancia de variables en Regresión Logística (coeficientes).  
   - Importancia de variables en Random Forest (feature importance).  

4. **Conclusiones estratégicas**  
   - Identificación de factores de riesgo y protectores.  
   - Recomendaciones de negocio basadas en los hallazgos del modelo.  

---

## 📊 Resumen de resultados

- **Mejor modelo:** Regresión Logística (Accuracy ≈ 0.80, Recall ≈ 0.53).  
- **Factores más influyentes en el churn:**  
  - Baja antigüedad (**tenure**).  
  - Altos **cargos mensuales**.  
  - **Contrato mes a mes**.  
  - **Internet con fibra óptica**.  
  - Métodos de pago como **cheque electrónico** y facturación digital.  

📌 **Conclusión principal:** Los clientes con baja permanencia y cargos altos son los más vulnerables al churn. Estrategias de retención deben enfocarse en los **primeros 6 meses**, con incentivos hacia contratos de mayor permanencia y mejora en la experiencia del servicio de fibra óptica.  

---

## 📦 Librerías utilizadas

- pandas  
- numpy  
- scikit-learn  
- imbalanced-learn  
- matplotlib  
- seaborn  

---

## 🔗 Relación con la primera parte

📍 En la **Parte 1** se realizó un **análisis exploratorio y descriptivo** del churn (EDA).  
📍 En esta **Parte 2** se implementaron **modelos predictivos** para anticipar qué clientes presentan mayor riesgo de abandono.  

Ambas fases se complementan: primero se exploraron los factores asociados y luego se construyeron modelos capaces de predecirlos.

---
