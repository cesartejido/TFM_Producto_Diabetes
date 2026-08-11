# 🩺 Clasificación de enfermos diabéticos mediante Machine Learning

📌 Trabajo de Fin de Máster – Máster en Inteligencia Artificial (CEMP)

## 👤 Autor

Julio César Tejido González
Máster en Inteligencia Artificial – CEMP

## 🧑‍🏫 Director del TFM

Cristian Rodríguez

Tutor colaborador: Marta Gabriela Tudorache

## 🎯 Resumen

Este proyecto desarrolla un modelo de aprendizaje automático para la clasificación de pacientes con diabetes a partir de variables clínicas, con el objetivo inicial de apoyar el diagnóstico de pacientes concretos y el objetivo final de plantear una solución potencialmente desplegable en un entorno hospitalario real. El trabajo cubre el ciclo completo: limpieza y preprocesamiento de datos, análisis exploratorio, entrenamiento y comparación de varios algoritmos, evaluación clínica de resultados y un plan de implantación hospitalaria (regulatorio, económico y de gestión del cambio).

## 📄 Introducción

La diabetes es una de las enfermedades crónicas con mayor prevalencia a nivel mundial, y su detección temprana tiene un impacto directo en la calidad de vida de los pacientes y en los costes sanitarios asociados a complicaciones no tratadas a tiempo. Este proyecto explora hasta qué punto un modelo de Machine Learning entrenado sobre variables clínicas básicas puede apoyar esa detección temprana, y qué implicaciones tendría llevar una solución así a un hospital real.

## 📊 Conjunto de datos

Se emplea el dataset **Pima Indians Diabetes** (n=768, 8 variables predictoras + variable objetivo), disponible públicamente en el [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/34/diabetes). Todas las pacientes son mujeres de la etnia Pima; los valores de 0 en varias columnas (Glucosa, Presión arterial, Grosor de piel, Insulina, IMC) representan datos faltantes y no valores clínicos reales, lo cual se documenta y se trata explícitamente durante el preprocesamiento.

## 📂 Metodología

El proyecto sigue las fases propuestas por la guía del TFM (alineadas con CRISP-DM): definición del problema, recolección y preparación de datos, análisis exploratorio, selección de modelos y entrenamiento, validación y evaluación, optimización, e implementación. Todo el desarrollo se realiza en Python sobre Google Colab, utilizando un `Pipeline` de scikit-learn para evitar fuga de datos entre los conjuntos de entrenamiento y prueba, validación cruzada estratificada con búsqueda de hiperparámetros, e imputación robusta de valores faltantes.

## 🧪 Modelos evaluados

Se comparan varios algoritmos de clasificación (Regresión Logística, Random Forest, SVM, KNN), seleccionando el umbral de decisión final mediante análisis de la curva precision-recall, priorizando la sensibilidad clínica sobre la exactitud global.

## ✅ Conclusiones

*(Se completará al finalizar el desarrollo del modelo.)*

## 📁 Estructura del repositorio

```
data/          Dataset original y diccionario de variables
notebooks/     Notebooks de Google Colab (EDA, preprocesamiento, modelado y evaluación)
src/           Scripts de Python del pipeline final
figures/       Gráficas exportadas para la memoria del TFM
models/        Modelo entrenado final
```

## 🔗 Enlaces relacionados

- Memoria completa del TFM (PDF): *enlace pendiente*
- Dataset original: https://archive.ics.uci.edu/dataset/34/diabetes
