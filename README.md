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

## Resultados:
Se logró desarrollar un modelo que puede clasificar dígitos manuscritos con una precisión satisfactoria. Además, el modelo fue capaz de sintetizar nuevos dígitos que representan visualizaciones "promedio" de cada clase. A continuación, se presentan los resultados de las métricas de interés (Accuracy, Recall y F1-score), así como la matriz de confusión evaluadas sobre los datos de test.

- Matriz de confusión:
![image](https://github.com/bdrinconp/ml_mnist/assets/63571645/f49976bf-d54e-45c9-b73a-0343795d9d20)

- Métricas de interés:
![image](https://github.com/bdrinconp/ml_mnist/assets/63571645/b4a27094-e977-4eb9-bc2f-779ca9ce6b40)
