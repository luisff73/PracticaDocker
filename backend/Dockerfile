# Etapa de construcción Dockerfile backend
FROM php:8.1-alpine

RUN apk update && apk add --no-cache \
    bash \
    autoconf \
    gcc \
    g++ \
    make \
    libc-dev \
    re2c \
    mysql-client \
    pkgconf \
    && rm -rf /var/cache/apk/*

# Instala las extensiones PDO y PDO MySQL
RUN docker-php-ext-install pdo pdo_mysql
WORKDIR /app
COPY . .

# Instala cualquier dependencia de PHP si es necesario, por ejemplo:
RUN docker-php-ext-install pdo pdo_mysql

# Copia el script wait-for-it.sh y dale permisos de ejecución
COPY wait-for-it.sh /usr/local/bin/wait-for-it
RUN chmod +x /usr/local/bin/wait-for-it

EXPOSE 8000

# Define el comando de inicio, utilizando wait-for-it para asegurarse de que MySQL esté listo
CMD sh -c "wait-for-it mysql_contenidor:3306 -- php -S 0.0.0.0:80 -t /app"

