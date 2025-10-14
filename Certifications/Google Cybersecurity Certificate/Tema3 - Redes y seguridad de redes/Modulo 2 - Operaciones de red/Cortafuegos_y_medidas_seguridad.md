# Cortafuegos y medidas de seguridad de redes

### Firewall

Es un dispositivo de seguridad de red que monitorea el tráfico hacia y desde su red. Permite el tráfico o lo bloquea basándose en un conjunto definido de reglas de seguridad, cómo el filtrado de puertos, que bloquea o permite ciertos números de puerto para limitar la comunicación no deseada. A continuación veremos los diferentes tipos que hay: 

    - Firewall de hardware: Inspecciona cada paquete de datos antes de que se le permita entrar en una red

    - Firewall de software: Realiza las mismas funciones que un firewall de hardware, pero no es un dispositivo físico. En su lugar es un programa instalado en el PC o servidor. Analizará todo el tráfico recibido por ese PC y si se usa en un servidor protegerá todos los dispostivos conectados al servidor. Tiene menos costo que uno de hardware pero al tratarse de un programa puede añadir cierta carga de proceso a los dispositivos individuales. 

    - Firewall en la nube: Son firewalls alojados por un proveedor de servicios en la nube. Las organizaciones pueden configurar las reglas del firewall en la interfaz del proveedor de servicios en la nube y el firewall realizará operaciones de seguridad en todo el tráfico entrante antes de que llegue a la red de la organización. 

Todos estos firewalls pueden funcionar de dos maneras, que son: 

    - Con estado: Firewalls que realizan un seguimiento de la información que pasa a través de ellos y filtra proactivamente las amenazas. Analiza el tráfico de red para para encontrar comportamientos sospechosos e impide que entren a la red. 

    - Sin estado: Firewalls que se basan en reglas predefinidas y no llevan un registro de la información de los paquetes de datos. Sólo actúa según reglas preconfiguradas establecidas por el administrador del firewall. Estas reglas le dicen al firewall que aceptar y que rechazar. Un firewall sin estado no almacena información analizada y tampoco descubre tendencias sospechosas cómo si lo hace uno con estado. Por ello se considera que estos firewalls sin estado no son tan seguros. 

Ahora ya hay firewalls de nueva generación cómo los NGFW que son más seguros que uno con estado. No solo proporcionan inspección con estado del tráfico entrante y saliente, sino que también realiza más funciones de seguridad en profundidad como inspección profunda de paquetes y protección contra intrusiones.