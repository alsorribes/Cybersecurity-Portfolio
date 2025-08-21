# Registros y herramientas SIEM


### Registros

Es un registro de eventos que ocurren en los sistemas y redes de una organización. Existen tres fuentes de registro que son:

- **Registro de firewall:** Registro de las conexiones establecidas para el tráfico entrante de Internet. También incluye las solicitudes salientes a Internet desde dentro de la red.

- **Registro de red:** Registro de todos los dispositivos que entran y salen de la red. También registra las conexiones entre los dispositivos y los servicios de la red.

- **Registro de servidor:** Registro de eventos relacionados con servicios como sitios web, correos electrónicos o archivos compartidos. Incluye acciones como solicitudes de inicio de sesión, contraseña y nombre de usuario. 

Al monitorear todos estos registros los equipos de seguridad pueden identificar las vulnerabilidades y las posibles violaciones de datos gracias a las herramientas SIEM.


### SIEM

Estas herramientas proporcionan visibilidad en tiempo real, monitoreo y análisis de eventos y alertas automatizadas. También almacena todos los datos de registro en una ubicación centralizada. Aumentan la eficacia y ahorran tiempo porqué indexan i minimizan la cantidad de registros que un profesional debe revisar y analizar manualmente. Es importante destacar que estas herramientas tienen que configurarse según las necesidades de cada organización. 


### Paneles SIEM: 

Presentan información sobre tu cuenta o ubicación en un formato fácil de entender. Gracias a esto, se puede acceder a la información de seguridad fácilmente en forma de tablas y gráficos. Proporcionan un resumen completo de los datos relacionados con la seguridad y también proporcionan a la parte interesada diferentes métricas.

- **Métricas:** Son atributos técnicos, como el tiempo de respuesta, la disponibilidad y la tasa de fallos que se utilizan para evaluar el rendimiento de una app de software. Se pueden mostrar distintas métricas o datos relevantes para los miembros de la organización según el panel SIEM que más les convenga. 


### Herramientas SIEM más comunes

Primero hay que destacar los dos tipos de herramientas SIEM que nos podemos encontrar, que son:

- **Autoalojadas:** Requieren que las organizaciones instalen, operen y mantengan la herramienta utilizando su propia infraestructura física. Son gestionadas por el departamento de IT de la organización y son ideales para mantener el control físico sobre los datos confidenciales.

- **Nube:** Son mantenidas y gestionadas por los proveedores de SIEM, lo que las hace accesibles a través de Internet. Este tipo de herramientas SIEM son ideales para organizaciones que no quieren invertir en crear y mantener su propia infraestructura.

- **Híbrida:** Algunas organizaciones utilizan una combinación de las dos, así pueden aprovechar las ventajas de la nube y mantener el control físico de los datos confidenciales.


Ahora vamos a centrarnos en herramientas SIEM reales. Hablaremos de las siguientes:

- **Splunk Enterprise:** Herramienta autoalojada que se utiliza para retener, analizar y buscar datos de registro en una organización para proporcionar información de seguridad y alertas en tiempo real. 

- **Splunk Cloud:** Herramienta alojada en la nube que se utiliza para recopilar, buscar y monitorizar datos de registro. Es útil para organizaciones que ejecutan entornos híbridos o solo en la nube. 

- **Chronicle:** Herramienta nativa de la nube diseñada para retener, analizar y buscar datos. Proporciona supervisión de registros, análisis de datos y recopilación de datos. Al ser nativa, está diseñada específicamente para aprovechar al máximo las capacidades de computación de la nube, como la disponibilidad, flexibilidad y escalabilidad. 


Una vez visto unas de las diferentes herramientas SIEM reales que hay, vamos a ver los paneles que componen cada herramienta. Empezaremos con Splunk, que consta de los siguientes paneles: 

- **Panel de postura de seguridad:** Diseñado para los centros de operaciones de seguridad ya que muestra las últimas 24h de los eventos y tendencias relacionados con la seguridad de una organización y permite a los profesionales determinar si la infraestructura y las políticas están funcionando según lo previsto. Los analistas usan este panel para supervisar e investigar las amenazas potenciales en tiempo real.

- **Panel de resumen ejecutivo:** Analiza y supervisa la salud general de la organización a lo largo del tiempo. Los analistas de seguridad podrian usar este tablero para proporcionar estadísticas de alto nivel a las partes interesadas, como generar un resumen de los incidentes de seguridad y las tendencias durante un período de tiempo.

- **Panel de revisión de incidentes:** Permite a los analistas identificar patrones sospechosos que pueden producirse en caso de incidente. Ayuda resaltando los elementos de mayor riesgo que necesitan atención inmediata.

- **Panel de análisis de riesgos:** Ayuda a identificar el riesgo para cada objeto de riesgo (un ordenador, por ejemplo). Muestra los cambios en el comportamiento relacionados con el riesgo, como el inicio de sesión de un usuario fuera de las horas normales de trabajo. Un analista puede usar este panel para analizar el impacto potencial de las vulnerabilidades en los recursos críticos.


Ahora pasaremos a revisar los paneles de la herramienta SIEM Chronicle. Hay que destacar que Chronicle permite recopilar y analizar datos de registro en función de un recurso específico, un nombre de dominio, un usuario y una dirección IP. Una vez visto esto, vamos a proceder con sus paneles que son los siguientes: 

- **Panel de estadísticas empresariales:** Identifica nombres de dominio sospechosos en los registros, conocidos como **Indicadores de compromiso (IOC)**. Cada resultado se etiqueta con una puntuación de confianza para indicar la probabilidad de una amenaza. También dispone de un nivel de gravedad que indica la importancia de cada amenaza para la organización. Un analista usaría este panel para monitorizar los intentos de inicio de sesión de un dispositivo poco habitual. 

- **Panel de ingestión de datos y salud:** Muestra el número de registros de eventos, las fuentes de registro y las tasas de éxito de los datos que se están procesando en Chronicle. Un analista podría usar este panel para asegurarse de que las fuentes de registro están correctamente configuradas y que los registros se reciben sin errores. 

- **Panel de coincidencias IOC:** Indica las principales amenazas, riesgos y vulnerabilidades para la organización. Los profesionales utilizan este tablero para observar los nombres de dominio, las direcciones IP y los IOC de los dispositivos a lo largo del tiempo con el fin de detectar tendencias para después enfocarse en las amenazas de mayor prioridad. 

- **Panel principal:** Muestra un resumen de alto nivel de la información relacionada con la actividad de ingestón de datos, alertas y eventos de la organización a lo largo del tiempo. Se usa para poder acceder a una cronología de los eventos de seguridad.

- **Panel de detección de reglas:** Proporciona estadísticas relacionadas con los incidentes de mayor incidencia, gravedad y detecciones a lo largo del tiempo. Un analista puede usar este panel para acceder a una lista de todas las alertas activadas por una regla de detección específica. Después, usan estas estadísticas para ayudar a gestionar los incidentes habituales y establecer tácticas de mitigación mejoradas.

- **Panel general de inicio de sesión de usuario:** Proporciona información sobre el comportamiento de acceso de los usuarios en toda la organización. Los profesionales usan este panel para cceder auna lista de todos los eventos de inicio de sesión de los usuarios para identificar actividades inusuales.