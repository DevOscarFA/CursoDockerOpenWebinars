# Curso de Docker
## Que es Docker
* Virtualización a nivel de S.O.
* Aislamiento de recurso a nivel de Kernel (cgroups, namespaces).
* Flexibilidad y portabilidad.
* Enfocado a sistemas altemente distribuidos.

## Iniciar con Docker
Para realizar la instalación de docker en cualquier sistema operativo debemos realizar los pasos que estan en el siguiente enlace [Get startted docker](https://docs.docker.com/get-started/).

## Conceptos iniciales
### Docker engine
Docker engine es la aplicación cliente servidor y tiene tres componentes.
* Demonio de docker.
* Una rest api que nos permite comunicarnos con el demonio de docker.
* Una interfaz de línea de comandos con la que usamos el servicio de docker.

### Registro de docker 
El registro de docker es un servicio que permite almacenar imágenes.

### Imagenes
* Plantilla de solo lectura.
* Sistema de ficheros y parámetros listos para ejecutar.
* Basadas en sistemas operativos Linux.

### Contenedores
* Instancia de una imagen.
* Es un directorio dentro del sistema, similar a los jail root.
* Pueden ser: ejecutados, reiniciados, parados entre otros.

## Construir imagenes propias
* Crear y configurar un fichero Dockerfile
* [Referencia de docker file](https://docs.docker.com/engine/reference/builder/#dockerfile-reference)
* Construir la imágen con el comando docker build

## Docker networking
Docker por defecto crea 3 tipos de redes:
* bridge (driver bridge). Red por defecto
* host (driver overlay)
* none

``` [powershell]
docker network ls
 ```