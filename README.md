# practica6
La url de la practica 6 es la siguiente:
      https://github.com/antoniobm1/practica6.git
      
##Instalacion de MYSQL y de NGINX
En esta practica crearemos 2 maquinas:
      -1 Front-end que sera con el servidor web NGINX
      -1 back-end que sera con la base de datos de MYSQL y PHP

## Instalacion de MYSQL y PHP
Instalaremos el back-end igual que hicimos en la practica 3 mediante el script subido en este repositorio

### Configuramos el php-fpm
Es recomendable realizar un cambio en la directiva de configuración cgi.fix_pathinfo por cuestiones de seguridad. Editamos el siguiente archivo de configuración:
```
sudo nano /etc/php/7.2/fpm/php.ini
```
Buscamos la directiva de configuración cgi.fix_pathinfo que por defecto aparece comentada con un punto y coma y con un valor igual a 1 y lo cambiamos a 0.

#Cambiamos el achivo config.php
Añadimos la ip de nuestro back-end para enlazarlo

##Instalacion de NGINX
Instalamos NGINX con el script correspondiente de instalacion y sus paquetes

##Configurar Nginx para usar php-fpm
Editamos el archivo de configuración /etc/nginx/sites-available/default

Ya estaria lista la practica

