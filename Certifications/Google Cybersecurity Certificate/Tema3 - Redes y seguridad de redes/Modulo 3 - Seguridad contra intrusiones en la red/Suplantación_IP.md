# Suplantación de IP

Es un ataque de red que se realiza cuando un atacante cambia la IP de origen de un paquete de datos para hacerse pasar por un sistema autorizado y obtener acceso a una red. En estos ataques, el atacante se hace pasar por alguien que no es para comunicarse a través de la red con la computadora objetivo y superar las reglas del firewall que pueden impedir el tráfico externo.

Algunos ataques de de suplantación de IP más comunes son:

- **Ataques en ruta:** Ataque en el que el atacante se coloca en medio de una conexión autorizada e intercepta o altera los datos en tránsito. Los atacantes obtienen acceso a la red y se interponen entre dos dispositivos para luego rastrear la información del paquete para saber las direcciones IP y MAC de los dispositivos que se comunican. Una vez tienen esta información, pueden fingir ser cualquiera de estos dispositivos.

- **Ataque de repetición:** Ataque de red que se realiza cuando un atacante intercepta un paquete de datos en tránsito y lo retrasa o lo repite en otro momento. Un paquete retrasado puede provocar problemas de conexión entre los equipos de destino y un atacante puede tomar una transmisión de red enviada por un usuario autorizado y repetirla mas adelante para hacerse pasar por dicho usuario. 

- **Ataque de pitufos:** Es una combinación de un ataque DDoS y un ataque de suplantación de IP. El atacante detecta la dirección IP de un usuario y lo inunda de paquetes. Esto satura el equipo de destino y puede provocar la caída de un servidor o toda una red. 

Para poder proteger la red de estos ataques la mejor manera es usar el cifrado de los datos para que nadie pueda leerlos y el uso de firewalls para proteger contra la suplantación de IP.