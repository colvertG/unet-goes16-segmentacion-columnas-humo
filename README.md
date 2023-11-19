# Repositorio de tesis: Modelo de segmentación semántica de columnas de humo derivadas de incendios forestales en México

## Descripción:
Este repositorio alberga los resultados y el código asociado a la tesis que aborda el desafío de la segmentación semántica de columnas de humo provocadas por incendios forestales en México, utilizando imágenes satelitales del satélite GOES-16 y aprendizaje profundo.

## Descripción General
Este repositorio presenta los resultados de una investigación centrada en la detección y segmentación de incendios forestales utilizando imágenes del satélite GOES-16. Los logros obtenidos representan un avance significativo en la capacidad de monitoreo y predicción de incendios forestales, con implicaciones directas en la gestión y mitigación de estos eventos devastadores.

## Construcción de la Base de Datos
Se recopilaron y segmentaron manualmente 1061 imágenes de incendios forestales capturadas por el satélite GOES-16. Esta segmentación manual generó máscaras precisas de las regiones de humo, sirviendo como conjunto de datos de referencia para el entrenamiento, evaluación y prueba de los modelos.

El desafío de la limitada cantidad de datos se abordó mediante la implementación de la técnica de aumento de datos. Esta estrategia diversificó el conjunto de datos aplicando transformaciones como rotaciones, recortes y cambios de brillo a las imágenes originales y sus máscaras de segmentación. La técnica demostró mejorar la generalización y reducir el sobreajuste.

El conjunto de datos final está disponible para su descarga en [Kaggle](https://www.kaggle.com/datasets/colvertgomez/goes16-wildfires-smoke-plumes-dataset).

## Resultados y Métricas
El modelo final alcanzó un índice de Jaccard (IoU) de 0.8252 y un coeficiente Dice de 0.9042 en el conjunto de prueba, indicando una precisión sustancial en la superposición entre las regiones de humo predichas y las máscaras de referencia. La métrica de precisión alcanzó un valor de 0.9898.

## Conclusión
Los resultados demuestran el éxito de la metodología aplicada para la detección y segmentación de columnas de humo de incendios forestales en imágenes del satélite GOES-16. Estos avances ofrecen una vía para un monitoreo más efectivo y la mitigación temprana de los impactos de los incendios forestales.

