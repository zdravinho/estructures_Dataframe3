# Predicción de Clases de Vinos

Este proyecto tiene como objetivo construir y evaluar modelos de clasificación que pueden predecir correctamente la clase de vinos a partir de un conjunto de características químicas.

## Descripción de los datos
Los datos provienen del conjunto de datos de reconocimiento de vinos, que contiene los resultados de un análisis químico de vinos cultivados en una misma región de Italia pero derivados de tres diferentes cultivares. La base de datos contiene las cantidades de 13 componentes químicos encontrados en cada uno de los tres tipos de vinos.

Las características son las siguientes:

Alcohol
Ácido málico
Ceniza
Alcalinidad de la ceniza
Magnesio
Fenoles totales
Flavonoides
Fenoles no flavonoides
Proantocianinas
Intensidad del color
Matiz
OD280/OD315 de vinos diluidos
Prolina
El objetivo es predecir la clase del vino, que puede ser 1, 2 o 3.

## Preprocesamiento de los datos
Antes de entrenar los modelos, los datos fueron preprocesados. Esto incluyó la división de los datos en conjuntos de entrenamiento y prueba, y la estandarización de las características. La estandarización es importante porque muchos algoritmos de aprendizaje automático son sensibles a la escala de las características.

## Modelos de clasificación
Se entrenaron dos modelos de clasificación: un árbol de decisión y una máquina de vectores de soporte (SVM). Ambos modelos se entrenaron utilizando sus parámetros por defecto y luego se optimizaron utilizando la búsqueda de cuadrícula para encontrar la mejor combinación de parámetros.

Los modelos se evaluaron utilizando la precisión (la proporción de predicciones correctas) y la matriz de confusión, que muestra la distribución de las predicciones correctas e incorrectas. Además, se utilizó la validación cruzada para obtener una estimación más robusta de la precisión del modelo.

## Ingeniería de características
Se aplicó la selección de características para reducir la dimensionalidad de los datos y eliminar las características menos informativas. Esto no sólo puede mejorar el rendimiento del modelo, sino que también puede hacer que el modelo sea más fácil de interpretar y más eficiente desde el punto de vista computacional.

## Resultados
Tanto el árbol de decisión como el SVM lograron una alta precisión en la clasificación de los vinos. La precisión de los modelos fue aún más alta después de la optimización de los parámetros y la selección de características.

En general, este proyecto demuestra cómo se pueden construir y optimizar modelos de clasificación para predecir con precisión las clases de vinos a partir de sus características químicas.
