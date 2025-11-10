# Ataques de denegación de servicio (DoS)

Un ataque DoS es un ataque que tiene como objetivo una red o un servidor y lo inunda de tráfico de red. Su objetivo es interrumpir las operaciones comerciales de una organización al saturar la red de ella, enviando tanta información a un dispositivo de red para que se bloquee y no pueda operar con normalidad. Todo esto puede provocar pérdidas de tiempo y dinero para las organizaciones. 

Hay otro tipo de ataque de denegación de servicio que son los ataques de denegación de servicio distribuido o DDoS. Es un tipo de ataque que utiliza varios dispositivos o servidores para inundar la red objetivo con tráfico de red no deseado. Al usar varios dispositivos hay más posibilidades de que el tráfico enviado sature el servidor destino. 

A nivel de red hay tres ataques DoS muy comunes, que son:

- **Ataque de SYN flood:** Ataque DoS que simula la conexión TCP e inunda el servidor con paquetes SYN. Para entenderlo mejor repasaremos el proceso de este protocolo.

    - El dispositivo envía una solicitud SYN.
    - El servidor responde con un paquete SYN/ACK para confirmar la recepción de la solicitud del dispositivo y deja un puerto abierto.
    - Cuando el servidor recibe el paquete ACK final del dispositivo, se establece la conexión TCP.

Los atacantes pueden aprovechar este protocolo inundando un servidor con solicitudes de paquetes SYN. Si el número de solicitudes SYN es mayor que el número de puertos disponibles en el servidor, se saturará y no podrá funcionar con normalidad.
<br>

- **Ataque de inundación ICMP:** Este ataque usa el protocolo ICMP que son las siglas del Protocolo de Mensajes de Control de Internet. Este protocolo lo utilizan los dispositivos de Internet para informarse unos a otros sobre los errores de transmisión de datos en la red. Podemos pensar en ICMP como una solicitud de actualización de estado desde un dispositivo y, si hay algun problema con la red, devolverá mensajes de error. 

Este ataque se basa en enviar repetidamente paquetes ICMP a un servidor de red. Esto obliga al servidor a enviar un paquete ICMP y, con el tiempo, acabará consumiendo todo el ancho de banda haciendo que el servidor se bloquee. 
<br>

- **Ataque de ping of death:** Ataque DoS que se produce cuando un hacker hace ping a un sistema enviándole un paquete ICMP sobredimensionado de más de 64 KB, que es el tamaño máximo de un paquete ICMP. Esto provocará que el sistema se sobrecargue y se bloquee. 