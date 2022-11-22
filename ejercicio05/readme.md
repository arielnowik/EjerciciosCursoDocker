## Healthcheck
Este comando cumple la función de revisar si un contenedor sigue funcionando correctamente.
Sirve para detectar casos por ejemplo donde el servidor este en un loop infinito y no pueda aceptar conexiones a pesar de seguir ejecuntandose

## Onbuild

Agrega a la imagen una instrucción para ser ejecutada luego de iniciada la imagen para ser la base de la construcción de otra imagen distinta (Es decir luego del 'FROM' de otro Dockerfile que invoque a la imagen) 

## Volume

Crea un mount point en la imagen con un nombre determinado para poder mantener volumenes del host nativo o de otros contenedores.