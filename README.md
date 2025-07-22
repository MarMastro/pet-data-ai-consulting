# pet-data-ai-consulting

## Descripción del proyecto

Este repositorio es un portafolio de **Data & AI** aplicado a la predicción de adopción de mascotas. Utilizamos el dataset de [PetFinder.my Adoption Prediction](https://www.kaggle.com/c/petfinder-adoption-prediction) para realizar un Análisis Exploratorio de Datos (EDA), limpieza de outliers y exploración de variables clave.

## Objetivos

* Comprender la estructura y calidad del dataset.
* Limpiar valores atípicos (por ejemplo, recorte de Age a 25 años).
* Explorar variables relevantes (fotos, descripción, salud, etc.).
* Construir un modelo baseline con RandomForest.
* Mejorar el modelo con técnicas de balanceo (SMOTE) y texto (TF‑IDF).
* Optimizar hiperparámetros y preparar pipeline reproducible.

## Requisitos

* Python 3.9 o superior
* Paquetes: pandas, numpy, scikit-learn, imbalanced-learn, scipy, matplotlib, seaborn, jupyterlab
* (Opcional) API de Kaggle configurada con `kaggle.json`

## Pasos para reproducir el EDA

1. Clona el repositorio y crea un entorno virtual:

   ```bash
   git clone https://github.com/TuUsuario/pet-data-ai-consulting.git
   cd pet-data-ai-consulting
   python -m venv venv
   source venv/bin/activate  # o .\venv\Scripts\activate en Windows
   pip install -r requirements.txt
   ```
2. Descarga el dataset de Kaggle y descomprímelo en `data/`.
3. Inicia JupyterLab:

   ```bash
   jupyter lab
   ```
4. Ejecuta el Notebook `eda_petfinder.ipynb` para explorar y limpiar los datos.

## Resultados y métricas

A continuación se muestran las métricas de los principales modelos entrenados:

| Configuración                               | Accuracy | Macro F1 |
| ------------------------------------------- | -------- | -------- |
| Baseline (solo tabulares + class\_weight)   | 31.9 %   | 27.7 %   |
| + TF‑IDF (texto) + SMOTE                    | 41.2 %   | 37.7 %   |
| RF optimizado (RandomizedSearchCV reducido) | 40.7 %   | 36.0 %   |


---

*¡Gracias por visitar mi portafolio! Cualquier feedback o colaboración, no dudes en contactarme.*
