# ADD-NET-Plus: Técnica para la clasificación aplicada a neuroimágenes para el diagnóstico del Alzheimer.

Este estudio tiene como objetivo desarrollar una técnica avanzada de clasificación aplicada a neuroimágenes, orientada a mejorar el diagnóstico temprano y preciso del Alzheimer, facilitando así una intervención y tratamiento más efectivo.


En esta investigación, se ha mejorado significativamente la arquitectura ADD-NET , una red neuronal convolucional (CNN) empleada en la clasificación de neuroimágenes para el diagnóstico del Alzheimer, resultando en la creación de ADD-NET Plus.

Data set utilizado: [https://www.kaggle.com/datasets/sabari50312/fundus-pytorch](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images)

<h2>Resultados Preliminares:</h2>
Se llevaron a cabo dos experimentos clave para determinar dicha configuración.

En el primer experimento, se evaluó el desempeño del modelo a lo largo de 70 épocas. La elección de este número se fundamenta en el hecho de que la red neuronal alcanzó su mayor precisión en ese punto, sin presentar mejoras significativas al incrementar el número de épocas. De esta forma, se evitó el riesgo de sobreajuste, garantizando una mayor generalización del modelo.

El segundo experimento consistió en emplear la arquitectura ADD-NET Plus con las 70 épocas previamente establecidas, pero variando el número de capas densas, desde 1 hasta 5, y el porcentaje de dropout, desde el 20\% hasta el 50\%. Esto generó un total de 17 combinaciones posibles.

| Modelo       | Testing Accuracy | Testing Loss | Testing AUC | Testing F1-Score | Testing Recall |
|--------------|------------------|--------------|-------------|------------------|----------------|
| ADD-NET Plus | 98.63%           | 0.36%        | 99.95%      | 98.63%           | 98.45%         |
| ADD-NET      | 96.70%           | 0.46%        | 99.82%      | 98.61%           | 97.00%         |

