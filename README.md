# Clasificación de Dígitos Manuscritos (MNIST) con Naive Bayes

## Objetivo:
Este proyecto busca implementar un clasificador Naive Bayes para el conjunto de datos de dígitos manuscritos MNIST. Se pretende entender y aplicar los conceptos de probabilidad condicional y independencia condicional para clasificar imágenes de dígitos manuscritos.

## Descripción del Dataset:
El conjunto de datos MNIST contiene imágenes de dígitos manuscritos (del 0 al 9) en blanco y negro, normalizados y centrados. Cada imagen tiene un tamaño de 28x28 píxeles.

## Metodología:
Carga de Datos:
Se cargan las imágenes y las etiquetas del dataset MNIST.

## Preprocesamiento:
Las imágenes se binarizan utilizando diferentes umbrales, convirtiendo los píxeles en valores binarios (0 o 1), representando el color blanco o negro respectivamente.

## Implementación de Naive Bayes:
Se implementa el clasificador Naive Bayes, que se basa en el cálculo de probabilidades condicionales y la asunción de independencia condicional entre los píxeles dada la clase del dígito. Se calcula la probabilidad de cada píxel dado cada dígito y se utilizan estas probabilidades para clasificar nuevas imágenes.

## Validación Cruzada y Selección de Hiperparámetros:
Se realiza una validación cruzada para seleccionar el mejor umbral de binarización. El rendimiento del modelo se evalúa mediante el cálculo del accuracy en conjuntos de validación.

## Síntesis de Nuevos Dígitos:
Se genera un nuevo dígito sintético utilizando las probabilidades condicionales aprendidas por el modelo. Este nuevo dígito representa una visualización de un dígito "promedio" basado en las probabilidades condicionales de cada píxel.
