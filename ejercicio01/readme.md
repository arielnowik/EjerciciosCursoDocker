## Ejercicio 1 Para ejecutar el website

docker run --name my-website -v C:/Users/anowik/docker_test:/usr/share/nginx/html:ro -d -p 8080:80 nginx
8aa9941fdc20ed96200bb8be6f96cf7ad8e9b63b19942eaf43073ce592d6bfa3

Se coloca el archivo test.html en la carpeta docker_test de C:/Users/anowik