# Actividad 05 — Clustering Jerárquico, PCA (Eigenfaces) y NMF

Repositorio con la resolución de la Actividad 05 del curso de Aprendizaje de Máquina. Se abordan tres problemas de aprendizaje no supervisado usando `scikit-learn`.

## 📁 Contenido del repositorio

| Notebook | Descripción |
|---|---|
| [`Clustering_Jerarquico.ipynb`](./Clustering_Jerarquico.ipynb) | Clustering jerárquico aglomerativo sobre el dataset **20 Newsgroups**, comparando los criterios de linkage `ward`, `complete` y `average`. |
| [`Olivetti_Faces_PCA.ipynb`](./Olivetti_Faces_PCA.ipynb) | Sistema de reconocimiento facial basado en **Eigenfaces (PCA)** + SVM sobre el dataset **Olivetti Faces**, sin uso de redes neuronales. |
| [`NMF_Recomendacion_Articulos.ipynb`](./NMF_Recomendacion_Articulos.ipynb) | Sistema de **recomendación de artículos** periodísticos usando **NMF** + similitud de coseno, sobre el dataset BBC News Summary. |

El informe completo en PDF con la explicación detallada de los tres casos se encuentra en `/informe/Informe_Actividad05.pdf`.

## 🧩 Caso A — Clustering Jerárquico (20 Newsgroups)

- **Dataset:** subconjunto de 7 categorías de 20 Newsgroups (4011 documentos).
- **Pipeline:** TF-IDF → TruncatedSVD (LSA, 100 componentes) → `AgglomerativeClustering`.
- **Linkages comparados:** `ward`, `complete`, `average` (evaluados con ARI, NMI y Silhouette Score).
- **Resultado:** `ward` fue el más exitoso (ARI = 0.121, NMI = 0.311), mientras que `complete` y `average` sufrieron un efecto de encadenamiento (chaining effect).

## 👤 Caso B — Eigenfaces (PCA + SVM)

- **Dataset:** Olivetti Faces (400 imágenes, 40 personas, 64x64 px).
- **Pipeline:** PCA (100 componentes, 94% varianza explicada) → SVM (`GridSearchCV` sobre kernel y C).
- **Resultado:** Accuracy de **97%** en el conjunto de prueba, sin usar redes neuronales.

## 📰 Caso C — Recomendador de Artículos (NMF)

- **Dataset:** BBC News Summary (2225 artículos, 5 categorías).
- **Pipeline:** TF-IDF → NMF (5 tópicos) → similitud de coseno sobre la matriz de tópicos `W`.
- **Resultado:** temas interpretables (deportes, política, negocios, entretenimiento, tecnología) y recomendaciones coherentes por temática.

## 🛠️ Tecnologías utilizadas

- Python 3
- scikit-learn (`TfidfVectorizer`, `TruncatedSVD`, `AgglomerativeClustering`, `PCA`, `SVC`, `NMF`)
- pandas, numpy, matplotlib, scipy

## ▶️ Cómo ejecutar

1. Clonar el repositorio:
```bash
   git clone https://github.com/Flavio-zt/Aplicaciones_Modelos_Clustering_PCA_NMF.git
```
2. Abrir cada notebook en Google Colab o Jupyter.
3. Instalar dependencias si es necesario:
```bash
   pip install scikit-learn pandas numpy matplotlib scipy
```
4. Ejecutar las celdas en orden. El dataset 20 Newsgroups y Olivetti Faces se descargan automáticamente vía `scikit-learn`; el dataset BBC News Summary requiere montar Google Drive (ver notebook C).

## 👥 Equipo

- _Agregar nombres de los integrantes del equipo_

## 📄 Licencia

Uso académico — Actividad 05, curso de Aprendizaje de Máquina.
