# TFM_DetecciondeCancer
Comparativa de Modelos para Clasificación de Imágenes Histopatológicas
Este repositorio contiene los cuadernos de Jupyter utilizados para la implementación y evaluación de diversos modelos de aprendizaje profundo para la clasificación de imágenes histopatológicas, como parte de mi trabajo de fin de máster. Los modelos evaluados incluyen redes neuronales convolucionales, ResNet18, MobileNet, y Transformers de Visión, entre otros.

Estructura del Repositorio
Los cuadernos en este repositorio están organizados como sigue:

1.a cnn_cross_entropy-M.ipynb: CNN con función de pérdida de entropía cruzada, conjunto mediano.

1.a cnn_cross_entropy-S.ipynb: CNN con función de pérdida de entropía cruzada, conjunto pequeño.

1.b cnn_focal_loss-M.ipynb: CNN con función de pérdida focal, conjunto mediano.

1.b cnn_focal_loss-S.ipynb: CNN con función de pérdida focal, conjunto pequeño.

2.a resnet18.ipynb: Implementación y entrenamiento del modelo ResNet-18.

2.b mobilenet_finetuning.ipynb: Ajuste fino de MobileNet para la clasificación.

3.a ViTModel.ipynb: Implementación y evaluación de un Transformer de Visión (ViT).

4.a BagOfVisualWords.ipynb: Implementación del método Bag of Visual Words.


Organización de los Datasets

Este proyecto utiliza dos estructuras principales de datasets para facilitar diferentes enfoques en el entrenamiento y evaluación de modelos:

DatasetPaciente: Este es el dataset original que contiene subcarpetas organizadas por paciente. Cada subcarpeta incluye imágenes histopatológicas correspondientes a un paciente específico, lo que es útil para análisis donde la agrupación por paciente es relevante.

datasetsClases: Para facilitar el entrenamiento de modelos donde es crucial el balance y la distribución uniforme de clases, se ha creado una variante del dataset organizada por clases en lugar de por paciente. Este dataset está subdividido en tres subconjuntos: train, test, y val, cada uno conteniendo imágenes de las clases correspondientes. Este enfoque es especialmente útil para la validación y prueba de modelos de clasificación, asegurando que cada clase esté adecuadamente representada en todas las fases del entrenamiento y evaluación.

Dependencias

Este proyecto requiere Python 3.11.4 y las siguientes librerías de Python, que se pueden instalar con pip:


pip install numpy==1.24.0 torch==2.2.0 torchvision==0.17.0


Contacto

Si tienes alguna pregunta o necesitas más información, no dudes en contactarme.
