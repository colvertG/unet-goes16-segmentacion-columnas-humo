# Repositorio de tesis: Modelo de segmentación semántica de columnas de humo derivadas de incendios forestales en México

## Descripción general:
Este repositorio alberga los resultados y el código asociado a la tesis que aborda el desafío de la segmentación semántica de columnas de humo provocadas por incendios forestales en México, utilizando imágenes satelitales del satélite GOES-16 y una U-Net.

## Construcción de la Base de Datos
Se recopilaron y segmentaron manualmente 1061 imágenes de incendios forestales capturadas por el satélite GOES-16. Esta segmentación manual generó máscaras precisas de las regiones de humo, sirviendo como conjunto de datos de referencia para el entrenamiento, evaluación y prueba de los modelos.

El conjunto de datos final está disponible para su descarga en [Kaggle](https://www.kaggle.com/datasets/colvertgomez/goes16-wildfires-smoke-plumes-dataset).

## Resultados y Métricas
El modelo final alcanzó un índice de Jaccard (IoU) de 0.8252 y un coeficiente Dice de 0.9042 en el conjunto de prueba, indicando una precisión sustancial en la superposición entre las regiones de humo predichas y las máscaras de referencia. La métrica de precisión alcanzó un valor de 0.9898.

## Instrucciones de Uso
Para volver a entrenar el modelo se debe descargar el conjunto de dato correr el codigo ""
Para segmentar una imagen con el modelo ya entrenado, se de
