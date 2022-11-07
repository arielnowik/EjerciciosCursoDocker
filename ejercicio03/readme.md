## Revision de layers

Ejecutamos docker inspect nicopaez/passwordapi-java:java8-alpine

vemos que hay 4 layers

Ejecutamos previo pull 
docker inspect nicopaez/passwordapi-java:java8-fabric 

vemos que hay 9 layers

Por observación comparten una sola layer, la empezada en 

sha256:73046094....