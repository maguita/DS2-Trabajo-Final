# Predicción de siniestros viales en CABA

## Description
Modelo de regresión para predecir la cantidad de siniestros viales en la Ciudad de Buenos Aires para cada combinación de fecha, comuna y franja horaria.
El objetivo es identificar las zonas y momentos de mayor riesgo para priorizar controles y recursos de seguridad vial.

## Data
Se utilizan dos datasets públicos del sitio del Gobierno de l Ciudad de Buenos Aires
* [Siniestros viales](https://data.buenosaires.gob.ar/ar/dataset/victimas-siniestros-viales/resource/40ec993a-00ad-40e5-936f-0a25f8d2c90b)
* [Comunas de CABA](https://data.buenosaires.gob.ar/el/dataset/comunas)

## Dependencies
* Python 3.13
* Librerias listadas en `requirements.txt`
 
## How To
1. Clonar el repositorio: `git clone https://github.com/maguita/DS2-Trabajo-Final.git`
2. Instalar las dependencias: `pip install -r requirements.txt`
3. Abrir `Trabajo_final.ipynb` con Jupyter y ejecutar todas las celdas en orden.
 
  ## Repository structure
├── Datasets/
│   ├── siniestros_viales_hechos.csv
│   └── comunas.geojson
├── Trabajo_final.ipynb
├── requirements.txt
└── README.md
