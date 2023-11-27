# Repositorio de tesis: Modelo de segmentación semántica de columnas de humo derivadas de incendios forestales en México

## Descripción general:
Este repositorio alberga los resultados y el código asociado a la tesis que aborda el desafío de la segmentación semántica de columnas de humo provocadas por incendios forestales en México, utilizando imágenes del satélite GOES-16 y arquitectura de aprendizaje profundo U-Net.

## Construcción de la Base de Datos
Se recopilaron y segmentaron manualmente 1061 imágenes de incendios forestales capturadas por el satélite GOES-16. Esta segmentación manual generó máscaras precisas de las regiones de humo, sirviendo como conjunto de datos de referencia para el entrenamiento, evaluación y prueba de los modelos.

El conjunto de datos final está disponible para su descarga en [Kaggle](https://www.kaggle.com/datasets/colvertgomez/goes16-wildfires-smoke-plumes-dataset).

## Resultados y Métricas
El modelo final alcanzó un índice de Jaccard (IoU) de 0.8252 y un coeficiente Dice de 0.9042 en el conjunto de prueba, indicando una precisión sustancial en la superposición entre las regiones de humo predichas y las máscaras de referencia. La métrica de precisión alcanzó un valor de 0.9898.

| **Conjunto**  | **IoU** | **Dice** | **Precisión** |
| ------------- | ------- | -------- | ------------- |
| Entrenamiento | 0.8873  | 0.9403   | 0.9934        |
| Validación    | 0.8326  | 0.9086   | 0.9904        |
| Prueba        | 0.8252  | 0.9042   | 0.9898        |

## Instrucciones de Uso
Para reentrenar el modelo final, sigue estos pasos:
1. Descarga el conjunto de datos desde Kaggle.
2. Asegúrate de tener todas las bibliotecas requeridas instaladas en tu entorno.
3. Ajusta las direcciones en el código fuente para reflejar la ubicación de tus datos descargados.
2. Ejecuta el código de entrenamiento "" para actualizar el modelo con los nuevos datos.

Para utilizar el modelo entrenado:
1. Descarga los pesos del modelo desde el archivo designado.
2. Ajusta el código para apuntar al directorio de los pesos descargados.
3. Asegúrate de tener todas las bibliotecas requeridas instaladas en tu entorno.
4. Utiliza el código para segmentar nuevas imágenes y obtener predicciones basadas en el modelo previamente entrenado.

Los notebooks ubicados en el directorio /optim han sido creados para experimentar con diferentes conjuntos de hiperparámetros. Puedes explorar y ajustar estos notebooks según sea necesario para mejorar el rendimiento del modelo y adaptarlo a tus necesidades específicas.

## Ejemplo de segmentación:
Segmentaciones predichas por el modelo (azul), y segmentación manual (verde) de 20 imágenes aleatorias del conjunto de prueba.
![image](https://github.com/colvertG/unet-goes16-segmentacion-columnas-humo/assets/39036143/2b766700-9a5c-4cc4-8750-0d91c8d158cd)
