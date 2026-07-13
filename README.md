# Actividad 05 — Clustering Jerárquico, PCA (Eigenfaces) y NMF

Repositorio con la resolución de la Actividad 05 del curso de Aprendizaje de Máquina. Se abordan tres problemas de aprendizaje no supervisado usando `scikit-learn`.

## 📁 Contenido del repositorio

| Notebook | Descripción |
|---|---|
| [`Clustering_Jerarquico.ipynb`](./Clustering_Jerarquico.ipynb) | Clustering jerárquico aglomerativo sobre el dataset **20 Newsgroups**, comparando los criterios de linkage `ward`, `complete` y `average`. |
| [`Olivetti_Faces_PCA.ipynb`](./Olivetti_Faces_PCA.ipynb) | Sistema de reconocimiento facial basado en **Eigenfaces (PCA)** + SVM sobre el dataset **Olivetti Faces**, sin uso de redes neuronales. |
| [`NMF_Recomendacion_Articulos.ipynb`](./NMF_Recomendacion_Articulos.ipynb) | Sistema de **recomendación de artículos** periodísticos usando **NMF** + similitud de coseno, sobre el dataset BBC News Summary. |

# Aplicaciones de Modelos de Clustering Jerárquico, PCA y NMF

## Descripción

Este repositorio contiene el desarrollo de la **Actividad 05** del curso de Machine Learning, cuyo objetivo es comprender las aplicaciones de modelos de **Clustering Jerárquico**, **Análisis de Componentes Principales (PCA)** y **Factorización de Matrices No Negativas (NMF)** utilizando datasets proporcionados por la biblioteca **scikit-learn**.

A través de estos casos de estudio se analizan diferentes técnicas de aprendizaje no supervisado y reducción de dimensionalidad, aplicadas a problemas reales como el agrupamiento de documentos, el reconocimiento de rostros y los sistemas de recomendación.

---

## Objetivos

- Comprender el funcionamiento del Clustering Jerárquico.
- Aplicar PCA para la reducción de dimensionalidad y reconocimiento de rostros.
- Implementar NMF para la recomendación de artículos similares.
- Analizar e interpretar los resultados obtenidos en cada caso de estudio.

---

## Contenido del Repositorio

### Clustering_Jerarquico.ipynb

Implementación del algoritmo de **Clustering Jerárquico** utilizando el dataset **20 Newsgroups** de scikit-learn.

Se realiza:

- Carga y preprocesamiento del dataset.
- Vectorización del texto.
- Comparación de diferentes criterios de *Linkage*.
- Evaluación de resultados.
- Análisis de los grupos obtenidos.

---

### Olivetti_Faces_PCA.ipynb

Implementación de un sistema de reconocimiento de rostros mediante **PCA (Principal Component Analysis)** utilizando el dataset **Olivetti Faces**.

Se desarrolla:

- Carga del dataset.
- Aplicación de PCA.
- Obtención de Eigenfaces.
- Representación de imágenes.
- Reconocimiento y análisis de resultados.

---

### NMF_Recomendacion_Articulos.ipynb

Desarrollo de un sistema de recomendación de artículos utilizando **NMF (Non-negative Matrix Factorization)**.

Incluye:

- Procesamiento del texto.
- Extracción de temas mediante NMF.
- Cálculo de similitud entre documentos.
- Recomendación de artículos relacionados.

---

## Tecnologías utilizadas

- Python
- Google Colab
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- SciPy

---

## Datasets utilizados

- **20 Newsgroups Dataset**
- **Olivetti Faces Dataset**
- Dataset de artículos utilizado para el sistema de recomendación.

---

## Integrantes

- Flavio Zapana Ticona
- Integrante 2
- Integrante 3
- Integrante 4

---

## Docente

*(Nombre del docente)*

---

## Universidad

**Universidad Nacional del Altiplano – Puno**

Escuela Profesional de Ingeniería de Sistemas

---

## Licencia

Proyecto desarrollado con fines académicos.
