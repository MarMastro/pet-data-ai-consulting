# pet-data-ai-consulting

## Descripción del proyecto

Este repositorio es tu portafolio de **Data & AI** aplicado a la predicción de adopción de mascotas. Utilizamos el dataset de la competencia [PetFinder.my Adoption Prediction](https://www.kaggle.com/c/petfinder-adoption-prediction) para realizar un Análisis Exploratorio de Datos (EDA), limpieza de outliers y exploración de variables clave.

## Objetivos

* Comprender la estructura y calidad del dataset.
* Identificar patrones que expliquen la velocidad de adopción (`AdoptionSpeed`).
* Documentar hallazgos y pasos de limpieza.

## Requisitos

* Python 3.8 o superior
* Entorno virtual (venv o conda)
* Librerías:

  ```bash
  pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab
  ```

## Estructura del repositorio

```
pet-data-ai-consulting/
├── data/                   # Datos raw descargados de Kaggle
│   ├── train.csv
│   ├── test.csv
│   └── ...
├── notebooks/              # Jupyter notebooks de EDA y limpieza
│   ├── 01_EDA_petfinder.ipynb
│   └── 02_Cleaning_and_Visualization.ipynb
├── .gitignore
└── README.md               # Este archivo
```

## Pasos para reproducir el EDA

1. **Clonar el repositorio**

   ```bash
   git clone https://github.com/TuUsuario/pet-data-ai-consulting.git
   cd pet-data-ai-consulting
   ```

2. **Crear y activar el entorno virtual**

   ```bash
   python -m venv venv
   source venv/bin/activate    # Linux/macOS
   .\venv\Scripts\activate   # Windows PowerShell
   ```

3. **Instalar dependencias**

   ```bash
   pip install -r requirements.txt
   ```

4. **Descargar y colocar los datos**
   - Opción manual: descarga el ZIP desde Kaggle y extrae `train.csv` y `test.csv` en la carpeta `data/`.
   - Opción CLI Kaggle:

   ```bash
   kaggle competitions download -c petfinder-adoption-prediction -p data
   unzip data/petfinder-adoption-prediction.zip -d data
   ```

5. **Ejecutar JupyterLab**

   ```bash
   jupyter lab
   ```

   * Abre los notebooks en `notebooks/` y sigue las instrucciones de cada uno.

## Notebooks clave

* **01\_EDA\_petfinder.ipynb**: Inspección de estructura, nulos y distribuciones.
* **02\_Cleaning\_and\_Visualization.ipynb**: Tratamiento de outliers (recorte de edades), variables de texto y gráficos de adopción.

---


