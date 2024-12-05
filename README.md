# Taller3_Mlops

# Evaluación del Caso - Taller MLOps

## 1. Métrica de desempeño más importante
La métrica seleccionada para optimizar los modelos en este ejercicio fue el **Accuracy**. Esta métrica mide el porcentaje de predicciones correctas realizadas por el modelo, siendo una elección adecuada cuando el conjunto de datos está razonablemente balanceado, y el costo de los falsos positivos y falsos negativos es similar.

**Justificación del uso de Accuracy**:
- En este caso, el **Accuracy** permite evaluar de manera global el desempeño del modelo, dado que no se priorizó una clase específica (quiebra o no quiebra).
- Si bien métricas como el **Recall** o el **F1-score** serían más relevantes en escenarios donde el sesgo de clases es significativo o donde el costo de errores específicos es más alto, en este caso, el equilibrio en las predicciones globales es el objetivo principal.

---

## 2. Definición del mejor modelo
Tras la optimización y evaluación de varios modelos utilizando Optuna y MLflow, el mejor modelo identificado fue el **GradientBoostingClassifier**, con un **Accuracy** de **96.85%**.

### Hiperparámetros del modelo óptimo:
- Número de estimadores (`n_estimators`): 69
- Tasa de aprendizaje (`learning_rate`): 0.0639
- Profundidad máxima (`max_depth`): 7

Este modelo ofrece un balance ideal entre complejidad y desempeño, mostrando una capacidad sólida para generalizar a datos no vistos.

---

## 3. ¿Valdría la pena usar el mejor modelo en el día a día de una empresa/institución?
**Sí, valdría la pena usar este modelo**, considerando lo siguiente:

### Desempeño robusto:
- Con un **Accuracy** cercano al 97%, el modelo tiene un alto nivel de confianza para clasificar empresas en riesgo de quiebra correctamente.

---

## Conclusión
El modelo **GradientBoostingClassifier** es una solución efectiva para este problema, ofreciendo un desempeño destacado en términos de **Accuracy**. Su uso puede proporcionar ventajas significativas en la toma de decisiones empresariales, siempre que se realicen ajustes según el contexto específico del negocio o institución. Este modelo tiene el potencial de convertirse en una herramienta clave para mitigar riesgos financieros y optimizar recursos.

<img width="960" alt="MlopsTaller3" src="https://github.com/user-attachments/assets/9223b42f-c343-45a1-aa5e-1b0a8f6c47c1">



