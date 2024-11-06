# Practica Ubuntu Server

Cambiamos el nombre del servidor

![](./imagenes/Captura.PNG)

Configuramos la tarjeta de red accediendo a ```/etc/netplan/00-installer-config.yaml```

![](./imagenes/Captura2.PNG)

# Ubuntu cliente

Cambiamos el nombre del equipo en ```/etc/hostname``` y le asignamos una IP que pueda comunicarse con el servidor

![](./imagenes/Captura3.PNG)

Comprobamos que hace ping al servidor

![](./imagenes/Captura4.PNG)

# Windows Cliente

 Cambiamos el nombre del equipo

![](./imagenes/Captura5.PNG)

 Asignamos una IP que pueda comunicarse con el servidor

![](./imagenes/Captura6.PNG)

Comprobamos que tambien hace ping al servidor

![](./imagenes/Captura7.PNG)

# DHCP

Añadimos la IP que actuará de DHCP

![](./imagenes/Captura8.PNG)

Instalamos el servidor con ```apt-get install isc-dhcp-server```

Editamos el fichero ```/etc/default/isc-dhcp-server```

![](./imagenes/Captura10.PNG)

El fichero principal de configuración de DHCP es ```/etc/dhcp/dhcpd.conf.```
 Modificamos este archivo definiendo la subnet y el rango de IPs que se van a repartir a los clientes

![](./imagenes/Captura11.PNG)

Reiniciamos el servicio

![](./imagenes/Captura12.PNG)

Comprobamos que se asigna la IP en Windows y Ubuntu

![](./imagenes/Captura13.PNG)
![](./imagenes/Captura14.PNG)

Comprobamos el estado del servidor

![](./imagenes/Captura15.PNG)

![](./imagenes/Captura16.PNG)

Verificamos los leases en el servidor

![](./imagenes/Captura17.PNG)

Configuramos una reserva definiendo la MAC del cliente al que queremos que se le conceda y la IP que le queremos dar, y reiniciamos el server

![](./imagenes/Captura18.PNG)

Hacemos un ip renew y comprobamos que le ha dado la ip reservada

![](./imagenes/Captura19.PNG)

## Al apagar el servidor podremos comprobar que la configuración no cambia.












