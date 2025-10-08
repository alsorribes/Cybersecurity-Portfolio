# Componentes de la capa de red de comunicación 

### Operaciones en la capa de red

Las funciones en la capa de red organizan el direccionamiento y la entrega de los paquetes de datos a través de la red desde el dispositivo emisor hasta el dispositivo receptor. La dirección IP de destino está incluida en el encabezamiento de cada paquete de datos. Esta dirección se almacenará con fines de enrutamiento futuro en las tablas de enrutamiento a lo largo de la ruta de acceso del paquete hasta su destino. El encabezado también incluye otra información cómo la dirección IP de origen, el tamaño del paquete y qué protocolo se utilizará para su procesamiento. 

### Formato de un paquete IPv4

<p align="center">
  <img src="img/ipv4.png" alt="IPv4" width="600">
</p>

<br>
Un paquete IPv4 se compone de dos secciones, la cabecera y los datos:

- **Cabecera:** El formato del encabezado IPv4 viene determinado por el protocolo IPv4 e incluye la información de enrutamiento IP que los dispositivos utilizan para dirigir el paquete. El tamaño oscila entre 20 y 60 bytes. Los primeros 20 bytes son un conjunto fijo de información que contiene datos como la dirección IP de origen y destino, la longitud de la cabecera y la longitud total del paquete. El último conjunto de bytes puede oscilar entre 0 y 40. Además, dentro de esta cabecera podemos encontrar 13 campos que son:

    - Versión (VER): Componente de 4 bits que indica a los dispositivos receptores qué protocolo está utilizando el paquete. 

    - Longitud del encabezado IP (HLEN o IHL): HLEN es la longitud del encabezado del paquete. Indica dónde termina el encabezado del paquete y dónde comienza el segmento de datos.

    - Tipos de servicio (ToS): Los routers priorizan la entrega de paquetes para mantener la calidad del servicio en la red. Este campo proporciona al router esta información. 

    - Longitud total: Comunica la longitud total del paquete IP incluyendo la cabecera y los datos.

    - Identificación: Los paquetes IPv4 pueden tener hasta 65.535 bytes pero la mayoría de redes tienen un límite menor. En estos casos los paquetes se fragmentan en paquetes IP más pequeños. Este campo proporciona un identificador único para todos los fragmentos del paquete IP original, de forma que puedan ser reagrupados una vez lleguen a su destino.

    - Banderas: Proporciona al dispositivo de enrutamiento más información sobre si el paquete original ha sido fragmentado y si hay más fragmentos en tránsito.

    - Desplazamiento de fragmentación: El campo de offset de fragmentación indica a los dispositivos de encaminamiento a qué parte del paquete original pertenece el fragmento. 

    - Tiempo de vida (TTL): Impide que los paquetes de datos sean reenviados por los routers indefinidamente. Contiene un contador que se decrementa en uno a medida que pasa por cada router a lo largo de su ruta. Cuando el contador TTL llega a cero, el router que tiene el paquete en ese momento lo descarta y devuelve al remitente un mensaje de error ICMP Time Exceeded. 

    - Protocolo: Indica al dispositivo receptor qué protocolo se utilizará para el campo de datos del paquete. 

    - Suma de comprobación del encabezado: Contiene una suma de comprobación que puede utilizarse para detectar la corrupción del encabezado IP en tránsito. Los paquetes corruptos se descartan. 

    - Dirección IP origen: Dirección IP de origen es la dirección IPv4 del dispositivo emisor

    - Dirección IP destino: Dirección IP de destino es la dirección IPv4 del dispositivo receptor.

    - Opciones: Permite aplicar opciones de seguridad al paquete si el valor HLEN es superior a cinco. Este campo comunica estas opciones a los dispositivos de enrutamiento. 

- **Sección de datos:** La longitud de la sección de datos puede variar mucho en tamaño. Sin embargo, el tamaño máximo posible es de 65.535 bytes. Contiene el mensaje que se transfiere por Internet. 