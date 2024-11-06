# Practica Ubuntu Server

## Cambiar nombre del servidor
![Texto alternativo](./imagenes/Captura.PNG "Pie de imagen")

## Configuración de tarjeta de red asignando una IP para el servidor.
![Texto alternativo](./imagenes/Captura2.PNG "Pie de imagen")

## Ubuntu cliente
![Texto alternativo](./imagenes/Captura3.PNG "Pie de imagen")

![Texto alternativo](./imagenes/Captura4.PNG "Pie de imagen")

# Windows Cliente

## Cambiamos el nombre del equipo
![Texto alternativo](./imagenes/Captura5.PNG "Pie de imagen")

## Asignamos una IP que pueda comunicarse con el servidor
![Texto alternativo](./imagenes/Captura6.PNG "Pie de imagen")

![Texto alternativo](./imagenes/Captura7.PNG "Pie de imagen")

# DHCP

## Añadimos la IP que actuará de DHCP
![Texto alternativo](./imagenes/Captura8.PNG "Pie de imagen")

## Instalamos el servidor con **apt-get install isc-dhcp-server**

## Editamos el fichero **/etc/default/isc-dhcp-server**
![Texto alternativo](./imagenes/Captura10.PNG "Pie de imagen")

## El fichero principal de configuración de DHCP es **/etc/dhcp/dhcpd.conf.** 
## Modificamos este archivo definiendo la subnet y el rango de IPs que se van a repartir a los clientes
![Texto alternativo](./imagenes/Captura11.PNG "Pie de imagen")

## Reiniciamos el servicio
![Texto alternativo](./imagenes/Captura12.PNG "Pie de imagen")

## Comprobamos que se asigna la IP en Windows y Ubuntu
![Texto alternativo](./imagenes/Captura13.PNG "Pie de imagen")
![Texto alternativo](./imagenes/Captura14.PNG "Pie de imagen")

## Comprobamos el estado del servidor
![Texto alternativo](./imagenes/Captura15.PNG "Pie de imagen")

![Texto alternativo](./imagenes/Captura16.PNG "Pie de imagen")

## Verificamos los leases en el servidor
![Texto alternativo](./imagenes/Captura17.PNG "Pie de imagen")

## Configuramos una reserva definiendo la MAC del cliente al que queremos que se le conceda y la IP que le queremos dar, y reiniciamos el server
![Texto alternativo](./imagenes/Captura18.PNG "Pie de imagen")

## Hacemos un ip renew y comprobamos que le ha dado la ip reservada
![Texto alternativo](./imagenes/Captura19.PNG "Pie de imagen")

## Al apagar el servidor podemos comprobar que la configuración no cambia.












