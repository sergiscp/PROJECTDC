Proyecto Ciencias de Datos
================

## Proyecto de ciencia de datos reproducible

Este proyecto se centra en el análisis de la base de datos CO2 and Greenhouse Gas Emissions,
publicada por Our World in data. La base de datos utilizada es abierta, permitiendo la trazabilidad y reproducción del proyecto.


### Objetivo General del proyecto:

- Explorar la evolución de las emisiones de dióxido de carbono de manera temporal y geográfica.

### Objetivos específicos:
- Comparar las emisiones en diferentes periodos, observando que tendencia de emisiones se observan
- Comparar las emisones entre países, y observar que países son los mayores emisores.
- Observar evolución del uso de fuente de combustión, responsables de las emisiones de CO2.

Los datos utilizados en el proyecto comprenden emisiones en el periodo comprendido entre 1750 y 2023.

Link a la base de datos:[Data on CO2 and Greenhouse Gas Emissions by Our World in Data](https://github.com/owid/co2-data.git)

[Our World in Data](https://github.com/owid/co2-data.git)


Versión de R utilizada:

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
Todos los materiales disponen de  archivos con Código y Output
- Base de datos .csv original
- Dashboard: presenta visualizaciones interactivas sobre las emisiones entre países
- Informe: principales resultados del proyecto
- Presentación: diapositivas simples de las conclusiones


### Cargar datos:

 Código para cargar datos si te encuentras en la raíz de la carpeta  del proyecto:

 ```r
df<-read.csv("Datos/Base_Datos_Original.csv")
```

 Código para importar datos si el archivo está en una carpeta distinta de Datos:

```r
df<-read.csv("../Datos/Base_Datos_Original.csv")

```
Librerías necesarias para reproducir el proyecto, se pueden instalar con install.packages():
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

### Resultados del proyecto:

Las emisiones de CO₂ a nivel global muestran un crecimiento significativo durante los últimos 300 años.
A inicios de los años cincuenta (1950), y en un periodo de cincuenta años, las emisiones pasa de 50 mil (MtCO₂), a 20 mil (MtCO₂).
Este crecimiento a nivel global es significativo dado que no se muestran cambios  en el crecimiento de emisiones en los años anteriores
El crecimiento en emisiones, no disminuye en las posteriores décadas, por lo contrario, a partir sigue un incremento importante,
posteriormente de los años 2000 hacia adelante aún muestra un incremento más rápido. Estas emisiones incrementadas a lo largo del tiempo, están principalmente provocadas por la quema de combustibles fósiles.