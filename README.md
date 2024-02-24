# TAREA_FINAL
La tarea consiste en analizar una base de datos y poder predecir si un paciente tiene cancer o no.
Para lograrlo hacemos lo siguiente:
# Paso 1
- Importar las bibliotecas necesarias.
- Cargar y dividir el conjunto de datos en entrenamiento y prueba.
# Paso 2: Entrenamiento de los Modelos
- Inicializar y entrenar los modelos con el conjunto de datos de entrenamiento.
- Los modelos a evaluar son Regresión Logística, Random Forest  y Máquinas de Vectores de Soporte (SVM)
# Paso 3: Evaluación de los Modelos
- Utilizar la matriz de confusión y el informe de clasificación para evaluar cada modelo. La matriz de confusión proporciona una visión directa del rendimiento del modelo en términos de verdaderos positivos, falsos positivos, verdaderos negativos y falsos negativos.
- El informe de clasificación ofrece métricas detalladas como la precisión, la sensibilidad (recall), la especificidad (implícita) y el F1-score para cada clase, lo cual es crucial para entender cómo se comporta cada modelo.
# Paso 4: Decisión sobre el Mejor Modelo
- Sensibilidad (Recall): Esencial para enfermedades graves donde los falsos negativos pueden tener consecuencias significativas. El modelo con la mayor sensibilidad es preferible si el objetivo es asegurar que se identifiquen todos los casos positivos.
- Especificidad: Importante para reducir la carga de pruebas de seguimiento innecesarias en casos falsos positivos.
- Precisión y F1-Score: Proporcionan un equilibrio entre la precisión y la sensibilidad, útiles cuando se busca un modelo bien balanceado.
- Consideraciones Adicionales: Incluyen el costo asociado con los falsos positivos y falsos negativos, la facilidad de interpretación del modelo, y cualquier restricción operativa como el tiempo de predicción o la complejidad del modelo.
- Para poder decidir se toma en cuenta lo delicado de la información, por lo mismo, se hizo 3 pasos.
# Evaluacion del modelo
Paso 1: Primero analizamos la matriz de desiciones:
