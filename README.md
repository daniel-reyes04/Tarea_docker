# Tarea_docker
Tarea instalacion MongoDB

Construccion de la imagen:
Explicacion comandos:
nano Dockerfile: crea el DockerFile donde va a estar alijada la imagen
Dentro de este se escribe "FROM mongo:4.4 EXPOSE 27017" donde damos el comando de que utilice la version 4.4 de mongoDB y que exponga el puerto por defecto que utiliza mongoDB
NOTA:Se utiliza la version 4.4 de mongoDB ya que la version mas reciente de el motor de base de datos que es la 5.0 exige que soporte instrucciones AVX las cuales no soporta la maquina virtual.
docker build -t mi_mongo .: este crea una imagen llamada mi_mongo utilizando el dockerfile.
docker run -d --name base_daniel_mongoDB -p 27017:27017 mi_mongo: este crea un contenedor llamado base_daniel_mongoDB y lo inicia.

Contenedor ejecutandose:
Se ejecuta el comando docker ps para verificar el contenedor ejecutandose.

Evidencia de funcionamiento de base de datos

Nota: Las evidencias se encuentran adjuntas en esta carpeta
