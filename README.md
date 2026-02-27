[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/Linth84/EdVillalbaTelecomXParte2/blob/main/EdVillaba_Telecom_X_Parte_2.ipynb
)

# 📊 Telecom X – Predicción de Evasión de Clientes (Churn)

**Autor:** Armando Rene Cartagena Muñoz  
**Challenge:** Telecom X Parte 2 
**Programa:** Especialización en Data Science

---

## 🧠 Descripción del proyecto

Este proyecto corresponde a la segunda fase del análisis de Telecom X, en la cual se desarrolla un modelo predictivo de Machine Learning orientado a anticipar la evasión de clientes (churn).

A partir del conjunto de datos previamente depurado y analizado en la fase exploratoria, se construye un pipeline de modelado que permite estimar la probabilidad de cancelación del servicio.

El enfoque combina preprocesamiento estructurado, entrenamiento de modelos supervisados, evaluación con métricas apropiadas e interpretación de resultados desde una perspectiva de negocio.

---

## 🎯 Objetivos del proyecto

### Objetivo general

- Construir y evaluar modelos de clasificación capaces de predecir la evasión de clientes en Telecom X.

### Objetivos específicos

- Preparar los datos para su utilización en algoritmos de Machine Learning.

- Analizar el balance de clases y su impacto en el desempeño del modelo.

- Entrenar y comparar distintos modelos de clasificación.

- Evaluar el desempeño utilizando métricas adecuadas para problemas de churn.

- Interpretar la relevancia de las variables predictoras.

- Generar recomendaciones estratégicas basadas en los resultados obtenidos.

---

## 🧹 Preparación y preprocesamiento de datos

En esta etapa se realizaron las siguientes tareas:

- Las principales etapas de preprocesamiento incluyeron:

- Carga del dataset tratado en la fase anterior.

- Eliminación de variables irrelevantes (identificadores).

- Codificación de variables categóricas mediante One-Hot Encoding.

- Separación de variables numéricas y categóricas utilizando 'ColumnTransformer'.

- Evaluación del desbalance de clases.

- Aplicación de normalización únicamente en modelos sensibles a la escala.

- Este enfoque permitió estructurar un flujo de transformación coherente y reproducible.
---

## 🤖 Modelado y evaluación

Se entrenaron y compararon los siguientes modelos:

DummyClassifier (Baseline): modelo de referencia para establecer un punto mínimo de comparación.

Árbol de Decisión: modelo interpretable y no sensible a la escala.

Regresión Logística: modelo lineal sensible a la escala, seleccionado como modelo final por su equilibrio entre desempeño e interpretabilidad.

## 📊 Métricas utilizadas

- Accuracy

- Precision

- Recall

- F1-score

- Matriz de confusión (valores absolutos y normalizados)

- Dado el carácter estratégico del problema, se priorizaron métricas como Recall y F1-score, considerando la importancia de detectar clientes con riesgo de evasión.

---

## 📈 Importancia de las variables

A partir del modelo de Regresión Logística se analizó la contribución de las variables al proceso predictivo.

Principales hallazgos:

- Baja antigüedad incrementa la probabilidad de churn.

- Contratos de corto plazo presentan mayor riesgo.

- Determinadas configuraciones de servicios y niveles de cargos influyen en la decisión de cancelación.

- La permanencia prolongada y contratos de mayor duración actúan como factores protectores.

---

## 📌 Conclusiones

El modelo de Regresión Logística mostró el mejor desempeño general, logrando un equilibrio adecuado entre precisión y capacidad de detección.

El análisis confirma que la evasión no depende de un único factor, sino de la interacción entre variables contractuales, económicas y de comportamiento del cliente.

La implementación de modelos predictivos permite anticipar clientes en riesgo y diseñar estrategias de retención basadas en datos.

---

## 💡 Recomendaciones estratégicas

- Implementar estrategias de retención temprana para clientes con baja antigüedad.
- Incentivar la migración hacia contratos de mayor duración.
- Priorizar acciones comerciales sobre clientes identificados como de alto riesgo.
- Integrar el modelo predictivo como sistema de alerta temprana dentro del negocio.

---

## 🛠️ Tecnologías utilizadas

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  
- Google Colab  

---
