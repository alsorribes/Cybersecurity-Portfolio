# Protocolos de red

Son un conjunto de reglas que utilizan dos o más dispositivos de una red para describir el orden de entrega y la estructura de los datos. Sirven como instrucciones que acompañan a la información del paquete de datos. Estas instrucciones indican al dispositivo receptor qué debe hacer con los datos recibidos. 

Es importante saber que los protocolos desempeñan una función esencial en la comunicación de la red pero algunos de ellos tienen vulnerabilidades que los actores maliciosos pueden explotar. 

<br>

### Categorías de protocolos de red

- **Protocolos de comunicación:** Rigen el intercambio de información en la transmisión por red. Dictaminan cómo se transmiten los datos entre dispositivos y el momento de la comunicación. 

    - Protocolo de control de transmisión (TCP): Protocolo de comunicación a Internet que permite que dos dispositivos formen una conexión y transmitan datos. TCP utiliza un proceso de protocolo de enlace de tres vías. En primer lugar, el dispositivo envía una solicitud de sincronización (SYN) a un servidor. Después, el servidor responde con un paquete SYN/ACK para afirmar el recibo de la solicitud del dispositivo. Una vez que el servidor recibe el último paquete ACK del dispositivo, se establece una conexión TCP. --> Capa de transporte

    - Protocolo de datagramas de usuario (UDP): Protocolo no orientado a la conexión que no establece una conexión entre dispositivos antes de las transmisiones. Esto hace que sea menos fiable que el TCP aunque también significa que funciona bien para transmisiones que necesitan llegar a su destino rápidamente. Un uso que podría tener es el de enviar solicitudes DNS a servidores DNS locales. --> Capa de transporte

    - Protocolo de transferencia de hipertexto (HTTP): Protocolo que proporciona un método de comunicación entre clientes y servidores de sitios web. Se considera inseguro, por lo que está siendo sustituido en muchos sitios por la versión más segura que es HTTPS que utiliza encriptación de SSL/TLS para la comunicación. --> Capa de aplicación

    - Sistema de nombres de dominio (DNS): Protocolo que traduce los nombres de Internet en direcciones IP. Cuando un ordenador desea acceder al dominio de un sitio web utilizando su navegador de Internet, se envía la consulta a un servidor DNS dedicado. El servidor DNS busca la dirección IP que corresponde al dominio del sitio web. DNS normalmente usa UDP en el puerto 53. Hay que añadir que si la respuesta del DNS a una solicitud es grande, pasará a utilizar TCP. --> Capa de aplicación
<br>

- **Protocolos de gestión:** Se utilizan para supervisar y gestionar la actividad en una red. Incluyen protocolos para la notificación de errores y la optimización del rendimiento de la red. 

    - Protocolo simple de adminsitarción de red (SNMP): Protocolo de red utilizado para supervisar y gestionar los dispositivos de una red. SNMP puede restablecer una contraseña en un dispositivo de red o cambiar su configuración base. También puede enviar solicitudes a los dispositivos de red para obtener un informe sobre la cantidad de ancho de banda de la red que se está utilizando. --> Capa de aplicación

    - Protocolo de mensajes de control de Internet (ICMP): Protocolo de Internet que se utiliza entre dispositivos para informarse mutuamente de los errores de transmisión de datos a través de la red. Es utilizado por el dispositivo receptor  para enviar un informe al dispositivo emisor sobre la transmisión de datos. Se usa habitualmente como una forma rápida de solucionar problemas de conectividad y latencia de red mediante la emisión del comando "ping". --> Capa de Internet
<br>

- **Procolos de seguridad:** Garantizan que los datos se envían y reciben de forma segura a través de una red. Estos protocolos utilizan algoritmos de encriptación para proteger los datos en tránsito. 

    - Protocolo seguro de transferencia de hipertexto (HTTPS): Protocolo de red que proporciona un método seguro de comunicación entre clientes y servidores de sitios web. HTTPS es una versión segura de HTTP que utiliza la encriptación SSL/TLS (Secure Sockets Layer/Transport Layer Security) en todas las transmisiones para que los actores maliciosos no puedan leer la información contenida. HTTPS usa el puerto 443. --> Capa de aplicación

    - Protocolo seguro de transferencia de archivos (SFTP): Protocolo usado para transferir archivos de un dispositivo a otro a través de una red. SFTP usa Secure Shell (SSH), normalmente a través de puerto TCP 22. SSH utiliza el estándar de encriptación avanzada (AES) y otros tipos de encriptación para asegurar que los destinatarios no deseados no puedan interceptar las transmisiones. --> Capa de aplicación
<br>

A continuación vamos a ver algunos protocolos adicionales que nos vamos a encontrar en algunos casos pero que no acostumbran a ser tan relevantes cómo los vistos anteriormente, que son:

- **Traducciones de direcciones de red (NAT):** Los dispostivios de una red local tienen cada uno una dirección IP privada que utilizan para comunicarse directamente entre ellos. Sin embargo, para que los dispositivos con direcciones IP privadas puedan comunicarse con el Internet público, necesitan tener una única dirección IP pública que represente a todos los dispositivos de la LAN ante el público. Para los mensajes salientes, el router puede sustituir una dirección IP de origen privada por su dirección IP pública y hacer la operación inversa para las respuestas. Este proceso se conoce cómo traducción de direcciones de red (NAT) y normalmente requiere que un router o firewall esté configurado específicamente para realizar NAT. NAT forma parte de la capa 2 (capa de Internet) y la capa 3 (capa de transporte). 

- **Protocolo de configuración dinámica de host (DHCP):** Pertenece a la familia de protocolos de red de gestión. DHCP es un protocolo de capa de aplicación que se utiliza en una red para configurar dispositivos. Funciona con el router para asignar una dirección IP única a cada dispositivo y proporcionar las direcciones al servidor DNS y de la puerta de enlace predetermianda adecuados para cada dispositivo. Los servidores DHCP operan en el puerto UDP 67 mientras que los clientes DHCP lo hacen en el puerto UDP 68.

- **Protocolo de resolución de direcciones:** La dirección MAC es permanente porqué es única para la tarjeta de interfaz de red de un dispositivo. La dirección MAC se utiliza para comunicarse con dispositivos dentro de la misma red, pero a veces, la dirección MAC es desconocida. Por eso es necesario el protocolo de resolución de direcciones (ARP) que principalmente es un protocolo de la capa de acceso a la red que se utiliza para traducir las direcciones IP que se encuentran en los paquetes de datos a la dirección MAC del dispositivo de hardware. Cada dispositivo de la red ejecuta ARP y mantiene un registro de las direcciones IP y MAC coincidentes en una caché ARP. Este protocolo no tiene un número de puerto específico. 

- **Telnet:** Protocolo de la capa de aplicación que se utiliza para conectarse a un sistema remoto. Telnet envía toda la información en texto claro. Utiliza la linea de comandos para controlar otro dispositivo parecido a secure shell (SSH), lo que Telnet no es tan seguro. Utiliza el puerto TCP 23. 

- **Secure shell (SSH):** Se utiliza para crear una conexión segura con un sistema remoto. Este protocolo de capa aplicación proporciona una alternativa para la autenticación segura y la encriptación de la comunicación. SSH funciona a través del puerto TCP 22.

- **Protocolo de acceso a mensajes de Internet (IMAP):** Se utiliza para el correo electrónico entrante. Descarga las cabeceras de los correos electrónicos y el contenido del mensaje. El contenido también permanece en el servidor de correo electrónico, lo que permite a los usuarios acceder a su correo electrónico desde múltiples dispositivos. IMAP usa el puerto TCP 143 para el correo electrónico no cifrado y el puerto TCP 993 a través del protocolo TLS. 

- **Protocolo simple de transmisión de correo (SMTP):** Se usa para transmitir y encaminar el correo electrónico del remitente a la dirección del destinatario. SMTP funciona con el software del Agente de Transferencia de Mensajes (MTA), que busca en los servidores DNS para resolver las direcciones de correo electrónico en direcciones IP, con el fin de garantizar que los correos electróncios lleguen a su destino previsto. SMTP utiliza el puerto TCP/UDP 25 para los correos electrónicos no cifrados y para el spam de gran volumen y el puerto TCP/UDP 587 que utiliza TLS para los correos electrónicos cifrados.