# Clasificación Bancaria con Machine Learning y Redes Neuronales

🚧 Proyecto académico en desarrollo.

## Descripción

Análisis de datos de campañas de marketing bancario y desarrollo de modelos para clasificar la suscripción de clientes a depósitos a plazo.

Se compara una regresión logística, utilizada como baseline, con una red neuronal multicapa (MLP).

## Objetivo

Priorizar el recall de la clase positiva para reducir los falsos negativos e identificar una mayor proporción de los clientes que se suscriben.

## Metodología

- Análisis exploratorio de datos.
- Tratamiento de valores desconocidos e imputación con KNN.
- Codificación de variables categóricas y escalado.
- Implementación y comparación de técnicas de balanceo de clases: oversampling con SMOTE,   undersampling con Tomek Links y combinaciones de ambas.
- Entrenamiento de regresión logística y redes neuronales.
- Evaluación mediante recall, precision, F1-score y matriz de confusión.
- Análisis de importancia por permutación.

## Datos

Se utiliza el dataset Bank Marketing de UCI Machine Learning Repository, obtenido mediante la biblioteca `ucimlrepo`.

## Limitación de la variable `duration`

Se conservó la duración de la llamada por su aporte al recall en las pruebas realizadas. Sin embargo, este dato solo se conoce una vez finalizada la llamada.

Por lo tanto, las métricas de los modelos que incluyen esta variable corresponden a un escenario con duración conocida y no representan el rendimiento para seleccionar clientes antes de contactarlos. Para ese uso, se requiere una versión entrenada y evaluada sin `duration`.

## Organización

- `notebooks/`: notebook con el análisis y los modelos.
- `data/`: carpeta reservada para archivos de datos.
- `images/`: gráficos e imágenes del proyecto.

## Tecnologías

Python · pandas · NumPy · scikit-learn · TensorFlow/Keras · imbalanced-learn · Matplotlib · Seaborn

## Autoras

- Luciana Sol Parallela.
- Camila Belén González.

Trabajo académico realizado en la Universidad Nacional Guillermo Brown.