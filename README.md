# Predicción de siniestros viales en CABA

## Description
Modelo de regresión para predecir la cantidad de siniestros viales en la Ciudad de Buenos Aires para cada combinación de fecha, comuna y franja horaria.
El objetivo es identificar las zonas y momentos de mayor riesgo para priorizar controles y recursos de seguridad vial.

## Data
Se utilizan dos datasets públicos del sitio del Gobierno de la Ciudad de Buenos Aires.
* [Siniestros viales](https://data.buenosaires.gob.ar/ar/dataset/victimas-siniestros-viales/resource/40ec993a-00ad-40e5-936f-0a25f8d2c90b)
* [Comunas de CABA](https://data.buenosaires.gob.ar/el/dataset/comunas)

Los datasets se encuentran en la carpeta Datasets/ del repositorio, de la cual el notebook lee directamente.

## Dependencies
* Python 3.13
* Librerías listadas en `requirements.txt`
 
## How To
1. Clonar el repositorio: `git clone https://github.com/maguita/DS2-Trabajo-Final.git`
2. Instalar las dependencias: `pip install -r requirements.txt`
3. Abrir `Trabajo_final.ipynb` con Jupyter y ejecutar todas las celdas en orden.

## Results
El modelo final, XGBoost con objetivo Poisson, obtuvo en 2025 un Lift@5% de 2,64, lo que significa que el 5% de las combinaciones detectadas como de mayor riesgo registró en promedio 2,6 veces más siniestros que el promedio general.
Con las variables disponibles, el modelo obtuvo un rendimiento similar al baseline de promedio histórico por combinación. En la validación cruzada no logró superarlo, mientras que en los datos de prueba de 2025 obtuvo resultados ligeramente mejores. El detalle está en las conclusiones del notebook.
 
## Repository structure
```
├── Datasets/
│   ├── siniestros_viales_hechos.csv
│   └── comunas.geojson
├── Trabajo_final.ipynb
├── requirements.txt
└── README.md
```
