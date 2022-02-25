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
docker run --rm -p 8787:8787 -e USER=Test -e PASSWORD=Test -v [ruta]/rstudio:/home/Test/ jorgeo80/rocker

## Para subir a docker hub
docker push jorgeo80/rocker

## Para guardar la imagen de manera local
docker save jorgeo80/rocker > rocker.tar