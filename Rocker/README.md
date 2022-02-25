# Docker - RStudio

## Docker build
docker build -t jorgeo80/rocker .

## Imagenes
docker images 

## Quitar el contenedor despues de usarlo
docker run --rm

## Correr el Rocker
docker run --rm -p 8787:8787 -e USER=Test -e PASSWORD=Test jorgeo80/rocker

## Para ligar los archivos a la ruta
docker run --rm -p 8787:8787 -e USER=Test -e PASSWORD=Test -v [ruta]/rstudio:home/Test/folder jorgeo80/rocker