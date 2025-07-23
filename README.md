# Análisis Mundial del Consumo de Carne por País

Este proyecto analiza el consumo de carne per cápita en diferentes países, enfocándose especialmente en la carne de vacuno, área en la que trabajo. Usamos **Python** y **R** para análisis de datos y visualizaciones interactivas.

Este análisis integral combina estadística, clustering y visualizaciones interactivas para entender mejor el consumo de carne y su relación con indicadores socioeconómicos y ambientales. Puede orientar políticas públicas y estrategias de sostenibilidad en ganadería.



---

## Contenido

- [Objetivos](#objetivos)  
- [Metodología](#metodología)  
- [Resultados Clave](#resultados-clave)  
- [Tecnologías y Librerías](#tecnologías-y-librerías)  
- [Instrucciones para Reproducir el Análisis](#instrucciones-para-reproducir-el-análisis)  
- [Conclusión](#conclusión)  

---

## Objetivos

- Explorar patrones y relaciones entre consumo de carne, desarrollo económico y emisiones de CO₂.  
- Segmentar países según patrones de consumo mediante clustering.  
- Visualizar datos con mapas y gráficos interactivos.  
- Analizar tendencias en el consumo de carne de vacuno y su impacto ambiental.

---

## Metodología

### Preparación y limpieza de datos

- Carga y limpieza con **Pandas** y **GeoPandas**.  
- Conversión de nombres de países a continentes.  
- Corrección y unificación de códigos ISO para mapas.  
- Fusión (merge) de datasets para análisis conjunto.

### Análisis exploratorio

- Gráficos scatter de PIB per cápita vs consumo total de carne.  
- Cálculo de correlaciones lineales y logarítmicas.  
- Visualizaciones interactivas para evolución por país y continente.

### Segmentación por clustering

- Aplicación de K-means para agrupar países según consumo de diferentes tipos de carne.  
- Interpretación y descripción de clusters con características distintivas.

### Visualizaciones avanzadas

- Mapas interactivos con Plotly mostrando clusters y consumo por país.  
- Visualizaciones interactivas en R (Shiny) con treemaps por continente y país.

### Análisis ambiental

- Relación entre consumo de vacuno y emisiones de CO₂ per cápita.  
- Correlaciones entre PIB, consumo de carne y emisiones.  
- Conclusiones sobre impacto ambiental y económico.

---

## Resultados clave

- Correlación moderada entre PIB per cápita y consumo total de carne (r ~0.65), que mejora a r ~0.77 con transformaciones logarítmicas.  
- Identificación de 4 clusters claros de consumo:  
  - 🟢 Cluster 0: Alto consumo de pollo y pescado.  
  - 🟡 Cluster 1: Consumo moderado/bajo.  
  - 🔵 Cluster 2: Alto consumo general (cerdo y pollo).  
  - 🔴 Cluster 3: Alto consumo de otras carnes.  
- El consumo de vacuno ha disminuido en muchos países en la última década por razones ambientales, de salud y económicas.  
- Países más desarrollados emiten más CO₂ per cápita, pero el consumo de carne no es la causa principal; el desarrollo económico predomina.

---

## Tecnologías y Librerías utilizadas

**Python:**  
- pandas  
- numpy  
- geopandas  
- matplotlib  
- seaborn  
- plotly  
- scikit-learn  
- ipywidgets  

**R:**  
- tidyverse  
- shiny  
- plotly  
- treemapify  
- countrycode  

---

## Instrucciones para reproducir el análisis

1. Instalar dependencias de Python y R (desde consola R):

```bash
pip install rpy2 country_converter pycountry_convert geopandas plotly seaborn ipywidgets

install.packages(c("tidyverse", "plotly", "shiny", "readr", "curl", "httr", "treemapify"), repos="https://cloud.r-project.org/")




