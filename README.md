# Proyecto Backend en Docker

Este proyecto es una implementación de un backend utilizando Docker. 
Contiene los servicios de un servidor web PHP y una base de datos MySQL.
Se utiliza Docker Compose y Dockerfile. 
El objetivo es proporcionar un entorno de desarrollo completamente aislado y reproducible.
utilizando Docker y sobretodo la utilizacion de los recursos de DOCKERFILE y DOCKER COMPOSE.

## Estructura del Proyecto

## Tecnologías

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)


El proyecto contiene los siguientes archivos y carpetas:

- **config.php**: Configuración para la conexión a la base de datos MySQL.
- **index.php**: Página de inicio del backend.
- **item.php**: Script para interactuar con la base de datos y mostrar datos.
- **wait-for-it.sh**: Script para asegurarse de que el contenedor de MySQL esté listo antes de iniciar el backend.
- **docker-compose.yml**: Archivo para definir y ejecutar los contenedores Docker.
- **Dockerfile**: Archivo que define la imagen para el contenedor backend.
- **mysql**: Carpeta que contiene los archivos de inicialización de la base de datos MySQL.

## Requisitos

Antes de comenzar, asegúrate de tener los siguientes programas instalados:

- Docker: [Instrucciones de instalación](https://docs.docker.com/get-docker/)
- Docker Compose: [Instrucciones de instalación](https://docs.docker.com/compose/install/)

## Configuración

1. Clona el repositorio a tu máquina local:

   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   cd tu-repositorio
