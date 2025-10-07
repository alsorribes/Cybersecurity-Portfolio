# Modelo TCP/IP

Es un framework utilizado para visualizar cómo se organizan y transmiten los datos a través de una red.

- **TCP (Protocolo de control de transmisión):** Es un protocolo de comunicación de internet que permite a dos dispositivos formar una conexión y transmitir datos. Incluye unas instrucciones para organizar los datos, de forma que pueden enviarse a través de una red. 

- **IP (Protocolo de internet):** Enruta y direcciona paquetes de datos a medida que viajan entre dispositivos en una red. También encontramos la dirección IP que es una dirección para cada red privada. 

Cuando se envían y reciben paquetes de datos a través de una red, se les asigna un puerto. 

- **Puerto:** Ubicación basada en software que organiza el envío y recepción de datos entre dispositivos de una red. Dividen el tráfico de red en segmentos basados en el servicio que realizarán entre dos dispositivos.

Las computadoras que envían y reciben estos segmentos de datos saben cómo priorizar y procesar estos segmentos basándose en su número de puerto. Los paquetes de datos incluyen instrucciones que indican al dispositivo receptor que hacer con la información. Estas instrucciones vienen en forma de número de puerto, que permiten a las computadoras dividir el tráfico de red y priorizar las operaciones que realizarán con los datos.
<br>

### 4 capas del modelo TCP/IP

- **Capa de acceso a la red:** Se ocupa de la creación de paquetes de datos y su transmisión a través de la red. Corresponde al hardware físico implicado en la transmisión de la red cómo cableado y módems, por ejemplo. 

    - ARP: Es el protocolo de resolución de direcciones. Dado que las direcciones MAC se utilizan para identificar hosts en la misma red física, ARP es necesario para asignar direcciones IP a direcciones MAC para la comunicación de red local.

- **Capa de Internet:** Es la responsable de garantizar la entrega al host de destino, que normalmente se encuentra en una red diferente. Además, es donde se adjuntan las direcciones IP a los paquetes de datos para indicar la ubicación del emisor y del receptor. También determina que protocolo es responsable de entregar los paquetes de datos y garantiza la entrega al host de destino.

    - Protocolo de Internet (IP): IP envía los paquetes de datos al destino correcto y se basa en el Protocolo de control de transmisión/Protocolo de datagramas de usuario (TCP/UDP) para entregarlos al servicio correspondiente. Los paquetes IP permiten la comunicación entre dos redes que se encaminan entre la red emisaro hasta la red receptora. 

    - Protocolo de mensajes de control de Internet (ICMP): Comparte información sobre errores y actualizaciones del estado de los paquetes de datos. Es muy útil para detectar y solucionar errores de red. Además, transmite información sobre paquetes que se han perdido o que han desaparecido en tránsito, problemas con la conectividad de la red y paquetes redirigidos a otros routers. 

- **Capa de transporte:** Incluye protocolos para controlar el flujo de tráfico a través de una red. Estos protocolos permiten o deniegan la comunicación con otros dispositivos e incluyen información sobre el estado de la conexión. 

    - Protocolo de control de transmisión (TCP): Protocolo de comunicación de Internet que permite que dos dispositivos formen una conexión y transmitan datos. Garantiza que los datos se transmitan de forma fiable al servicio de destino. TCP contiene el número de puerto del servicio de destino previsto, que reside en el encabezado TCP de un paquete TCP/IP. 

    - Protocolo de datagramas de usuario (UDP): Protocolo no orientado a la conexión que no establece una conexión entre dispositivos antes de kas transmisiones. Lo utilizan aplicaciones a las que no les preocupa la fiabilidad de la transmisión. Los datos enviados a través de UDP no son objeto de un seguimiento tan exhaustivo como los enviados mediante TCP. Dado que UDP no establece conexiones de red, se utiliza sobre todo para aplicaciones sensibles al rendimiento que funcionan en tiempo real, como la transmisión de vídeo. 

- **Capa de aplicación:** Los protocolos determinan cómo los paquetes de datos interactuarán con los dispositivos receptores. Esta capa es la responsable de realizar las solicitudes de red o de responder a las peticiones además de definir qué servicios y aplicaciones de Internet pueden acceder los usuarios. Los protocolos mas comunes son: 

    - Protocolo de transferencia de hipertexto (HTTP)
    - Protocolo simple de transmisión de correo (SMTP)
    - Secure shell (SSH)
    - Protocolo de transferencia de archivos (FTP)
    - Sistema de nombres de dominio (DNS)
