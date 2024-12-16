# Repositorio para calcular Tabulados de la ENSU
![Estatus](https://img.shields.io/badge/Estatus-desarrollo-yellow)

## Introducción

En este repositorio encuentras código en R para realizar el procesamiento de los datos del Secretariado Ejecutivo del Sistema Nacional de Seguridad Pública (SESNSP) tanto víctimas como incidencia.

## Acerca de este proyecto

El Secretariado Ejecutivo del Sistema Nacional de Seguridad Pública (SESNSP) publica las cifras de incidencia delictiva, víctimas de delitos y unidades robadas, así como otro tipo de material referente a la seguridad pública de manera mensual en su sitio. Para mayor información y descarga de datos así como otro tipo de material visita el enlace: [SESNSP](https://www.gob.mx/sesnsp/acciones-y-programas/incidencia-delictiva-299891?state=published)


## Requerimientos
- [R (> 4.0)](https://www.r-project.org/)
- [Quarto](https://quarto.org/)  

Se recomienda instalar el IDE [Rstudio](https://www.rstudio.com/categories/rstudio-ide/), sin embargo es posible correr este proyecto con cualquier otro IDE donde la persona usuaria pueda utilizar `R`.

## Instrucciones de uso

Para ejecutar el código en este repositorio es necesario tener instalado el lenguaje de programación estadística `R`. El repositorio está ordenado de tal forma que todos los códigos se encuentran en la carpeta `procesamiento` y los datos se almacenan en la carpeta `datos`.

Primero debes realizar la descarga de los datos sobre víctmas en la página del Secretariado Ejecutivo del Sistema Nacional de Seguridad Pública [SESNP](https://www.gob.mx/sesnsp/acciones-y-programas/incidencia-delictiva-del-fuero-comun-nueva-metodologia?state=published) descomprimir el archivo colocar el archivo en la carpeta `datos/datos-originales` de este repositorio. 

Notarás que utilizó una ruta relativa y la función `here` para que no tengas que realizar ningún cambio en la ruta en el caso de tener quere replicar los resultados.

Posteriormente puedes utilizar algun de los archivos `quarto` para procesar los datos:

1. `femicidio.qmd` para calcular la cantidad de víctimas de feminicidio y homicidio doloso demujeres por año.
