# TelecomX_LATAM2.0
Descripción
Proyecto para predecir qué clientes de una empresa de telecomunicaciones tienen mayor probabilidad de cancelar el servicio (churn) y así apoyar decisiones de retención.
​
# Objetivos
1. Preparar y limpiar los datos para modelado (tratamiento de nulos, tipos, eliminación de ID y duplicados).
   ​
2. Transformar variables categóricas a numéricas (one‑hot encoding).
   
​3. Manejar el desbalance de clases en la variable Churn (uso de SMOTE).

​4. Entrenar y evaluar varios modelos de clasificación (Regresión Logística, KNN, SVM, Random Forest).

​5. Medir el desempeño con métricas estándar (accuracy, precisión, recall, F1, matriz de confusión).

​6. Identificar los factores que más influyen en la cancelación y proponer acciones de retención.
​

# Flujo del proyecto
Preparación de datos

Aplanado del JSON, renombrado de columnas, conversión de tipos, eliminación de nulos y ID_Cliente.
​
# Ingeniería de variables
Separación de X (features) e y (Churn).

One‑hot encoding de todas las variables categóricas (creación de X_encoded).

Balanceo y división de datos

División en train/test (70/30, estratificado).

Balanceo del entrenamiento con SMOTE.
​
# Modelado

Estandarización para modelos basados en distancia.

Entrenamiento de Regresión Logística, KNN, SVM (con datos escalados) y Random Forest (sin escalar).

Evaluación con accuracy, precisión, recall, F1 y matriz de confusión.
​
# Interpretación

Análisis de coeficientes (Regresión Logística) e importancia de variables (Random Forest).
​
Identificación de factores de riesgo (contrato mes a mes, baja antigüedad, fibra óptica, electronic check, uso intensivo de servicios digitales).
​
Propuesta de estrategias de retención (migrar a contratos de plazo, mejorar experiencia en fibra, incentivos por métodos de pago automáticos, paquetes para usuarios intensivos).
​
# Resultado clave

La Regresión Logística se selecciona como modelo principal por su mejor equilibrio entre desempeño y capacidad de generalización, y se propone usarla como motor de score de churn para priorizar acciones de retención sobre clientes de mayor riesgo.
