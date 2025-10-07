# Modelo OSI

Es un concepto estandarizado que describe las siete capas que utilizan los ordenadores para comunicarse y enviar datos a través de una red.

### Capa 7: Capa de aplicación

Su característica principal es la conexión del usuario a Internet a través de aplicaciones y solicitudes.Incluye procesos que implican directamente al usuario cotidiano y también incluye todos los protocolos de redes que las aplicaciones de software utilizan para conectar a un usuario a Internet. Algunos protocolos que podemos encontrar son: 

- HTTP
- HTTPS
- SMTP
- DNS

### Capa 6: Capa de presentación

Implica la traducción y encriptación de datos para la red. Esta capa añade y sustituye datos por formatos que puedan ser entendidos por las aplicaciones (capa 7) tanto en los sistemas emisores como en los receptores. Los procesos en la capa de presentación requieren el uso de un formato estandarizado. Algunas funciones de formateo que tienen lugar en esta capa incluyen la encriptación, la compresión y la confirmación de que el conjunto de códigos de caracteres puede ser interpretado en el sistema receptor. 

- SSL: Protocolo de encriptación de datos entre los servidores web y los navegadores web.

### Capa 5: Capa de sesión

Una sesión describe el momento en que se establece una conexión entre dos dispositivos. Una sesión abierta permite que los dispositivos se comuniquen entre ellos. Los protocolos de la capa de sesión mantienen la sesión abierta mientras se transfieren los datos y la terminan una vez se finaliza la transmisión. Esta capa también es responsable de la autenticación, la reconexión y el establecimiento de puntos de control durante una transferencia de datos y, si es interrumpida en algun momento, los puntos de control garantizan que la transmisión se retome en el último punto de control de la sesión cuando se reanude la conexión. Las funciones de esta capa son responder a las solicitudes de servicio de los procesos de la capa de presentación (capa 6) y enviar solicitudes de servicios a la capa de transporte (capa 4).

### Capa 4: Capa de transporte

Es la responsable de la entrega de datos entre dispositivos. Además de esto también se encarga de la velocidad de transferencia de datos, del flujo de la transferencia y de dividir los datos en segmentos más pequeños para facilitar su transporte. Este proceso de dividir grandes transmisiones de datos se llama segmentación. Estos segmentos tienen que volver a juntarse en su destino para que puedan ser procesados en la capa de sesión (capa 5). La velocidad y el ritmo de la transmisión también tienen que coincidir con la velocidad de conexión del sistema de destino. Los protocolos más comunes son:

- TCP
- UDP

### Capa 3: Capa de red

Supervisa la recepción de las tramas desde la capa de enlace de datos (capa 2) y las entrega al destino previsto. Los paquetes de datos permiten la comunicación entre dos redes ya que contienen direcciones IP que indican a los routers dónde enviarlos. 

### Capa 2: Capa de enlace de datos

Organiza el envío y la recepción de paquetes de datos dentro de una misma red. En esta capa se encuentran los conmutadores de la red local y las tarjetas de interfaz de red de los dispositivos locales. Los protocolos más comunes son:

- Protocolo de control de red (NCP)
- Control de enlace de datos de alto nivel (HDLC)
- Protocolo de control de enlace de datos síncrono (SDLC)

### Capa 1: Capa física

Corresponde al hardware físico que interviene en la transmisión de la red. Para que un paquete de datos pueda viajar a través de un cable ethernet, por ejemplo, necesita ser traducido a un flujo de 0s y 1s, después se recibe y a continuación pasa a niveles superiores del Modelo OSI. 