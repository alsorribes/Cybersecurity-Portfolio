# Zonas de seguridad

Son un segmento de una red que protege la red interna de Internet. Forman parte de una técnica de seguridad denominada segmentación de red que divide la red en segmentos y cada segmento tiene sus propios permisos de acceso y reglas de seguridad. Pueden controlar quien accede a los diferentes segmentos de una red y actúan como una barrera para las redes internas, mantienen la privacidad dentro de los grupos corporativos y evitan que los problemas se propaguen a toda la red. Un ejemplo sería el Wi-Fi público gratuito de un hotel, ya que el personal de ahí usará una red privada.

La red de una organización se clasifica en dos tipos de zonas de seguridad, que son:

- **Zona descontrolada:** Cualquier red fuera de control de la organización, como Internet. 

- **Zona controlada:** Es una subred que protege la red interna de la zona no controlada. Dentro de esta hay varios tipos:

    - **Zona desmilitarizada (DMZ):** Contiene servicios públicos que pueden acceder a Internet como servidores web, servidores proxy y servidores DNS que proporcionan direcciones IP a los usuarios de Internet. Actúa como un perímetro de red para la red interna ya que contiene servidores privados y datos de la organización.

    - **Zona restringida:** Protege la información altamente confidencial a la que solo pueden acceder los empleados con ciertos privilegios. 

Lo ideal en una red es que la DMZ esté situada entre dos firewalls. Uno para filtrar el tráfico fuera de la DMZ y el otro para filtrar el tráfico que entra en la red interna. Esto protege la red interna con varias líneas de defensa. Si hay una zona restringida también estaría protegida por otro firewall. 

Con todo esto, los ataques que penetran en la red DMZ no pueden propagarse a la red interna y los ataques que penetran en la red interna no pueden acceder a la zona restringida. 