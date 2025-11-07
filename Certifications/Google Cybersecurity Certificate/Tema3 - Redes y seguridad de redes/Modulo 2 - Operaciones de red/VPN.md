# Redes privadas virtuales (VPN)

Es un servicio de seguridad de red que cambia la dirección IP pública y oculta la ubicación virtual para poder mantener la privacidad de los datos mientras viajan por Internet para preservar la confidencialidad. 

Estos servicios realizan una encapsulación de los datos en tránsito que los protege empaquetando los datos confidenciales en otros paquetes de datos. Al estar cifrados podria parecer que los enrutadores no pudieran leer la dirección IP del paquete y no sabrian dónde enviarlo pero la encapsulación resuelve este problema. 

Los servicios VPN cifran sus paquetes de datos y los encapsulan en otros paquetes que los enrutadores pueden leer. Esto permite que las solicitudes de red lleguen a su destino mientras los datos siguen cifrados y que nadie pueda leerlos mientras circulan. Una VPN también usa un túnel cifrado entre el dispositivo y el servidor VPN. La encriptación no se puede hackear sin una clave criptográfica, por lo que nadie puede acceder a sus datos.

A continuación hablaremos de dos protocolos VPN, que son: 

- **VPN WireGuard:** Protocolo VPN de alta velocidad, con una encriptación avanzada, para proteger a los usuarios cuando acceden a Internet. Puede utilizarse tanto para VPNs de sitio a sitio como en VPNs de cliente-servidor. Es usado por mucha gente porque tiene más velocidad de descarga al utilizar menos líneas de programación. 

- **VPN IPSec:** Se usa este protocolo VPN para encriptar y autenticar los paquetes de datos con el fin de establecer conexiones seguras y encriptadas. Muchos sistemas operativos son compatibles con IPSec porque fue de los primeros en aparecer aunque eso implica que sea mas complejo que WireGuard. 