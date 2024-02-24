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
# Primer analisis matriz de desiciones:
Regresion Logica

![image](https://github.com/Danielsp1/TAREA_FINAL/assets/157714894/c4803c2f-654d-4a5b-a0e4-ea51766c77ca)

Random Forest

![image](https://github.com/Danielsp1/TAREA_FINAL/assets/157714894/150dda22-dfe8-4462-807a-7c36eaa6264c)

SVM

![image](https://github.com/Danielsp1/TAREA_FINAL/assets/157714894/5819bb3e-d759-4bf7-8157-441c2b6f6a57)

Podemos ver que SVM no tiene falsos negativos y es el único modelo que identificó correctamente todos los casos de cáncer (verdaderos positivos) sin errores (falsos negativos).
# Segundo analisis Muestras aleatorias:
Para este paso se selecciono 5 muestras aleatorias y se coparo con la etiqueta real, para poder comparar:

![image](https://github.com/Danielsp1/TAREA_FINAL/assets/157714894/a7667185-4a6e-422e-a090-72ba1d2d48c1)
 
Donde a pesar de la matriz de decisiones, se evidencia que SVM da menor tasa de probabilidad.

# Tercer analisis, 5 muestras con cancer vs 5 sin cancer
Para este paso se eligio 5 muestras donde sabiamos que tiene cancer vs 5 donde sabiamos que no tenian cancer:

![image](https://github.com/Danielsp1/TAREA_FINAL/assets/157714894/b73715ab-6f2d-4ff0-a24c-aed10884d81c)

# CONCLUSION FINAL
Dado tu el enfoque es minimizar falsos negativos, tanto la Regresión Logística como el Random Forest parecen ser las mejores opciones, sin embargo el Random Forest demostró no solo una alta sensibilidad sino también una excelente especificidad, lo que lo hace robusto tanto para identificar casos de cáncer como para confirmar la ausencia del mismo.




