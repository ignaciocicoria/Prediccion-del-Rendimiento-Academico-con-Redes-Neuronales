#  Predicción del Rendimiento Académico con Redes Neuronales

##  Descripción

En este problema se presenta un conjunto de datos que contiene información sobre el **rendimiento académico de estudiantes universitarios**, así como diversos factores que podrían influir en él.  
El objetivo es **construir un modelo de regresión utilizando redes neuronales** para predecir el **índice de rendimiento académico** de los estudiantes en función de las características proporcionadas.

---

##  Dataset

El dataset se encuentra en un repositorio de github.
El conjunto de datos incluye las siguientes variables:

| Variable | Descripción |
|-----------|-------------|
| **Hours Studied** | Número total de horas dedicadas al estudio por cada estudiante. |
| **Previous Scores** | Puntuaciones obtenidas en exámenes previos. |
| **Extracurricular Activities** | Participación en actividades extracurriculares (Sí / No). |
| **Sleep Hours** | Promedio de horas de sueño por día. |
| **Sample Question Papers Practiced** | Número de cuestionarios de muestra practicados. |
| **Performance Index** | *(Variable objetivo)* Índice de rendimiento académico general (10–100). Valores más altos indican mejor rendimiento. |

---

##  Objetivo

Construir un **modelo de regresión basado en redes neuronales** que pueda **predecir con precisión** el índice de rendimiento académico de los estudiantes.  
El modelo debe ser **entrenado y evaluado** aplicando técnicas adecuadas de validación y métricas de evaluación de regresión.

---

##  Metodología

1. **Exploración y preprocesamiento de datos**
   - Carga y análisis del dataset.
   - Limpieza y tratamiento de valores categóricos .
   - Normalización de las variables numéricas.
   - División del conjunto de datos en *train/test*.

2. **Construcción del modelo**
   - Implementación de una red neuronal densa (modelo secuencial).
   - Capas ocultas con activación *ReLU* y capa de salida *lineal*.
   - Entrenamiento con *Adam optimizer* y función de pérdida *MSE*.

3. **Evaluación**
   - Cálculo de métricas.
   - Análisis de errores y comparación entre valores reales y predichos.

---

##  Tecnologías Utilizadas

- **Python**
- **TensorFlow / Keras**
- **NumPy**
- **Pandas**
- **Matplotlib / Seaborn**
- **scikit-learn**

---

##  Resultados 

Se entrenaron y evaluaron dos modelos de regresión:

1. **Modelo completo:** utilizando todas las variables disponibles.  
   - **MAE:** 1.7632 (escala de 0 a 100).

2. **Modelo reducido:** utilizando solo las variables **"Previous Scores"** y **"Hours Studied"**.  
   - **MAE:** 1.9807 (escala de 0 a 100).
   - 
A pesar de que el segundo modelo presenta un error ligeramente superior, se considera **más conveniente**, ya que logra un desempeño muy similar utilizando un **conjunto reducido de características**, lo cual **simplifica el modelo** y **mejora su interpretabilidad**.

---
