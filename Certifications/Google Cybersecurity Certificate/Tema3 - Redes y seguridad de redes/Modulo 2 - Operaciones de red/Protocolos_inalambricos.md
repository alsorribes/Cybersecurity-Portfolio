# Evolución de los protocolos inalámbricos

Wi-fi hace referencia a un conjunto de estándares que definen la comunicación para las LAN inalámbricas. Los estándares y protocolos Wi-fi se basan en la familia 802.11 de estándares de comunicación de Internet determinados por el Instituto de Ingenieros Eléctricos y Electrónicos (IEEE). Por lo tanto, es posible que algunas veces veamos representado el Wi-fi cómo IEEE 802.11. Las comunicaciones Wi-fi están protegidas por protocolos de redes inalámbricas. 
<br>

### Privacidad equivalente por cable (WEP)

Es un protocolo de seguridad inalámbrica diseñado para proporcionar a los usuarios el mismo nivel de privacidad en las conexiones de redes inalámbricas que el que tienen en las conexiones de red por cable. Es el protcolo más antiguo de los estándares de seguridad inalámbrica. 
<br>

### Acceso Wi-fi protegido (WPA)

Se desarrolló este protocolo para mejorar el WEP y sustituirlo. Los fallos del WEP estaban en el propio protocolo y en cómo se utilizaba la encriptación. WPA abordó esa debilidad utilizando un protocolo llamado protocolo de integridad de clave temporal (TKIP). El algoritmo de encriptación WPA utiliza claves secretas más grandes que las WEP, lo que hace más difícil adivinar la clave por ensayo y error. 

WPA también incluye una comprobación de integridad del mensaje que incluye una etiqueta de autenticación del mensaje con cada transmisión. Si un actor malintencionado intenta alterar la transmisión de algún modo, la comprobación de integridad del mensaje de WPA identificará el ataque y rechazará la transmisión. 

A pesar de las mejoras, sigue siendo vulnerable. Los actores maliciosos pueden utilizar un ataque de reinstalación de claves (ataque KRACK) para desencriptar las transmisiones que utilicen WPA. Los atacantes pueden introducirse en el proceso de protocolo de enlace de autenticación WPA e insertar una nueva clave de encriptación en lugar de la dinámica asignada por WPA. Si establecen la nueva clave en todos ceros, es como si la transmisión no estuviera encriptada en absoluto. 

Debido a esto, WPA fue sustituido por una versión mejorada del protocolo denominada WPA2. 
<br>

### WPA2 y WPA3

- **WPA2:** WPA2 mejora a WPA utilizando el estándar de encriptación avanzada (AES). Además, también mejora el uso de TKIP de WPA. Utiliza el protocolo de código de autenticación de mensajes mediante cadena de bloques de cifrado en modo contador (CCMP), que proporciona encapsulación y garantiza la autenticación e integridad de los mensajes. Debido a su solidez, hoy en día se considera el estándar de seguridad para todas las transmisiones Wi-fi. Aún así, WPA2 sigue siendo vulnerable a los ataques KRACK y es por ello que apareció su sucesor que es WPA3.

- **WPA3:** WPA3 es un protocolo Wi-fi seguro y cada vez se usa más. Las diferencias que hay entre WPA2 y WPA3 son las siguientes:

    - WPA3 aborda la vulnerabilidad del protocolo de enlace de autenticación a los ataques KRACK, presente en WPA2.

    - WPA3 utiliza la Autenticación Simultánea de Iguales (SAE), un acuerdo de autenticación de contraseñas y uso compartido de claves de cifrado. Esto impide que los atacantes descarguen datos de las conexiones de redes inalámbricas a sus sistemas para intentar descodificarlos.

    - WPA3 ha aumentado la encriptación para que las contraseñas sean más seguras utilizando una encriptación de 128 bits.