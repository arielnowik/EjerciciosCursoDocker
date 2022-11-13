## Ejercicio 2

Descargamos la imagen de Nico:

docker run nicopaez/pingapp:3.0.0

![image](https://user-images.githubusercontent.com/79852716/201534973-eb7c6ab4-5d49-491e-af22-65ad58b5dbb2.png)

Creamos una imagen en docker hub:

![image](https://user-images.githubusercontent.com/79852716/201534966-9c83410b-3209-4c9d-b8b0-7f30bb45a80a.png)

Hacemos commit de la imagen que está corriendo a la imagen creada y la asignamos el host como tag

docker image tag anowik-testimage:lastest arielnowik/test-container-anowik:lastest
docker push arielnowik/test-container-anowik:test-tag

![image](https://user-images.githubusercontent.com/79852716/201534983-e826c8b1-a843-456e-b2b3-215dc15166b3.png)

Hacemos push

docker image push arielnowik/test-container-anowik:lastest

![image](https://user-images.githubusercontent.com/79852716/201534987-c7ab1222-ac6d-4c37-bd2c-35b789ff99b7.png)

Verificamos que la imagen publicada está en el repositorio
https://hub.docker.com/r/arielnowik/test-container-anowik/tags

![image](https://user-images.githubusercontent.com/79852716/201534991-a0fb8fe5-b108-425d-a0e8-68102f56196d.png)

Comando de pull: docker pull arielnowik/test-container-anowik:lastest

Eliminamos la imagen y probamos correrla descargandola de la nube:

docker rmi -f 2f7d14563135

![image](https://user-images.githubusercontent.com/79852716/201534998-cc5afa8a-7e75-4ee8-8e55-2c2059f9c80b.png)

docker run arielnowik/test-container-anowik:lastest

![image](https://user-images.githubusercontent.com/79852716/201535002-a4d109a3-beef-4962-ba5a-810a7596e55a.png)


