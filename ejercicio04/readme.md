## Generamos el dockerfile

FROM node:8
WORKDIR /usr/src/app
RUN git clone https://github.com/nicopaez/passwordapi /usr/src/app
RUN npm install --only production
EXPOSE 3000
CMD ["npm", "start"]

## Generamos la imagen

docker build -t "passwordapi" .

## Ejecutamos l.a imagen en un contenedor 

docker run -d -p 80 --name test passwordapidocker

## Comiteamos la imagen que esta en el contenedor para poder subirla al repositorio

docker container commit 19241e22a97d passwordapi:lastest

## Le asignamos un tag a la imagen para que este referencia correctamente al docker hub

docker image tag passwordapi:lastest newtonis/passwordapi:lastest

## Pusheamos la imagen al repositorio

docker push newtonis/passwordapi:lastest