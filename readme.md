# Proyecto de Análisis de Intensidades de Pastoreo – Atalaya

Este repositorio contiene el código, datos procesados y mapas generados para analizar las intensidades de pastoreo en la finca Atalaya mediante KDE (Kernel Density Estimation).  
El flujo principal del proyecto se ejecuta desde el notebook `mapas_kde_new.ipynb`.

---

## Estructura del proyecto

intensidades_atalaya/
│
├── atalaya/ # Información general de la finca  
├── cercados_atalaya/ # Geojson/QMD de los vallados  
├── data/ # Datos CSV procesados de posiciones  
├── geojson_guardados2/ # GeoJSON generados de salidas  
├── kde_grids/ # Grids KDE generales  
├── kde_grids_cercados/ # Grids KDE filtrados por vallados  
├── mapas_kde_html/ # Mapas HTML de intensidades  
├── mapas_kde_html_cercados/ # Mapas HTML por vallado  
  
├── mapas_kde_new.ipynb # Notebook principal del proyecto  
└── requirements.txt # Dependencias necesarias  


---

### Requisitos

Antes de ejecutar el notebook, instalar las librerías listadas en `requirements.txt`.

### Instalación de dependencias

Ejecutar desde una terminal en la carpeta raíz del proyecto:

```bash
pip install -r requirements.txt

Se recomienda usar un entorno virtual:
    python -m venv venv
    venv\Scripts\activate       # Windows
    source venv/bin/activate    # Linux / Mac
    pip install -r requirements.txt
```

Ejecución del notebook
Abrir el proyecto en VSCode o Jupyter Notebook.

Seleccionar el entorno donde se instalaron las dependencias.

Ejecutar el notebook: mapas_kde_new.ipynb
Los mapas y archivos generados se guardarán automáticamente en las carpetas correspondientes dentro del repositorio.

Salidas esperadas
    Mapas HTML mostrando intensidades de pastoreo por periodos
    KDE grids de densidad por finca y por vallado
    GeoJSON procesados