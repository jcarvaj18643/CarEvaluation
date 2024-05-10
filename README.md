# CarEvaluation

Comparación de Modelos de Clasificación: Random Forest vs K-Nearest Neighbors
Descripción General
Este documento proporciona un análisis comparativo de dos modelos de clasificación comúnmente usados, Random Forest y K-Nearest Neighbors (KNN), aplicados al conjunto de datos de clasificación de automóviles. La evaluación se basa en varias métricas de rendimiento, incluyendo matrices de confusión, reportes de clasificación y curvas ROC.

Conjunto de Datos
El conjunto de datos utilizado incluye varias características de automóviles, clasificadas en categorías como aceptable, bueno, inaceptable y muy bueno. Cada modelo intenta predecir estas categorías basándose en características como el precio de compra, mantenimiento, número de puertas, capacidad de personas, tamaño del maletero y seguridad.

Modelos Evaluados
Random Forest
Descripción: Un modelo de ensamble que utiliza múltiples árboles de decisión para tomar decisiones más precisas y robustas. Es bien conocido por su eficacia en la gestión de sobreajustes y su capacidad para manejar grandes conjuntos de datos con una alta dimensionalidad.
Resultados: El Random Forest demostró ser muy eficaz, con altas puntuaciones en precisión, recall y f1-score para casi todas las clases. Las curvas ROC reflejan una excelente capacidad de discriminación con AUCs cercanos o iguales a 1.0 para la mayoría de las clases.
K-Nearest Neighbors (KNN)
Descripción: Un modelo no paramétrico que clasifica los datos basándose en la similitud de las características con sus k vecinos más cercanos. Es simple pero efectivo, aunque su rendimiento puede depender significativamente de la elección del número de vecinos y la métrica de distancia utilizada.
Resultados: Aunque las curvas ROC indican una buena capacidad de discriminación, la precisión y el recall del modelo KNN fueron inconsistentes. Las clases con menos muestras, como 'good' y 'very good', mostraron bajos valores de precisión y f1-score, indicando dificultades en la clasificación efectiva de estas categorías.
Conclusión
En comparación, el modelo Random Forest superó al KNN en este conjunto de datos específico. Mostró una capacidad superior para manejar la variedad de clases y produjo resultados más equilibrados y precisos, lo que lo hace más adecuado para aplicaciones que requieren alta fiabilidad en la clasificación automática de características de automóviles.

Recomendaciones
Se recomienda utilizar el modelo Random Forest para futuras tareas de clasificación con este conjunto de datos. Para mejorar aún más el rendimiento, podrían explorarse ajustes en los parámetros del modelo, como el número de árboles en el bosque o la profundidad máxima de los árboles. Además, se sugiere realizar más pruebas con el modelo KNN ajustando el número de vecinos y la métrica de distancia para mejorar su precisión y recall.
