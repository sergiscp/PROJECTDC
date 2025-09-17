Proyecto Ciencias de Datos
================

## Proyecto de ciencia de datos reproducible

Este proyecto se centra en el analisis de la base de datos CO2 and Greenhouse Gas Emissions,
publicada por Our World in data.La base de datos utilizada es abierta, permitiendo la trazabilidad y repdouccion del proyecto.


### Objetivo General dep proyecto:

- Explorar la evolucion de las emisiones de dioxido de carbono de manera tempora y geografica.

### Ojectivos especificos:
- Comparar las emisiones en diferentes periodos, observando que tendencia de emisiones se observan
- Comparar las emisones entre paises, y observar que paises son los mayores emissores.
- Observar evolucion del uso de fuente de combustione, responsables de las emisiones de CO2.

Los datos utilizados en el proyecto comprenden emisiones en el periodo comprendido entr 1750 y 2023.

Link a la base de datos:[Data on CO2 and Greenhouse Gas Emissions by Our World in Data](https://github.com/owid/co2-data.git)

[Our World in Data](https://github.com/owid/co2-data.git)


Version de R utilizada:

```r

platform       x86_64-w64-mingw32               
arch           x86_64                           
os             mingw32                          
crt            ucrt                             
system         x86_64, mingw32                  
status                                          
major          4                                
minor          5.0                              
year           2025                             
month          04                               
day            11                               
svn rev        88135                            
language       R                                
version.string R version 4.5.0 (2025-04-11 ucrt)
nickname       How About a Twenty-Six  
```
### Contenidos del proyecto:
Todos los materialdes disponen de  archivos con Codigo y Output
- Base de datos .csv original
- Dashboard: presenta visualizaciones interactivas sobre las emisiones entre países
- Informe: principales resultados del proyecto
- Presentación: diapositivas simples de las conclusiones


### Cargar datos:

 Codigo para cargar datos si te encuentras en la raiz de lacarpeta  del proyecto:

 ```r
df<-read.csv("Datos/Base_Datos_Original.csv")
```

 Codigo para importar datos si el archivo esta en una carpeta distinta de Datos:

```r
df<-read.csv("../Datos/Base_Datos_Original.csv")

```
Librerias necesarias para reproducir el proyecto:
```r
library(flexdashboard)
library(plotly)
library(dplyr)
library(ggplot2)
library(DT)
library(rsconnect)
library(RColorBrewer)
library(shiny)
library(xtable)
library(knitr)
```

### Resultados principales del proyecto
