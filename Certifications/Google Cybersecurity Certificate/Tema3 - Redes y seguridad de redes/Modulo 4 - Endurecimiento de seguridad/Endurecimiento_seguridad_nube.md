# Endurecimiento de seguridad de la nube

### Gestión del aceso a la identidad (IAM)

Es un conjunto de procesos y tecnologías que ayuda a las organizaciones a gestionar las identidades digitales en su entorno. También autoriza la forma en que los usuarios pueden aprovechar los diferentes recursos de la nube

### Hipervisores

Abstrae el hardware del host del entorno del software operativo. Existen dos tipos: 

- **Hipervisor tipo uno:** Se ejecutan en el hardware del ordenador anfitrión. Ejemplo: ESXi de VMware

- **Hipervisor tipo dos:** Funcionan en el software del ordenador host. Ejemplo: Virtualbox

Los CSP suelen usar los de tipo uno y son los responsables de gestionar el hipervisor y otros componentes de virtualización. Las vulnerabilidades en los hipervisores o los errores de configuración pueden provocar escapes de máquinas virtuales (VM escapes). Un escape de VM es un exploit en el que un atacante obtiene acceso al hipervisor principal, potencialmente al ordenador host y otras VM

### Línea de base

Cubre cómo se configura y establece el entorno de la nube. Una línea de base es un punto de referencia fijo que puede utilizarse para comparar los cambios realizados en la nube. Una buena configuración y puesta a punto adecuadas pueden mejorar muchísimo la seguridad y el rendimiento de un entorno de nube.

### Criptografía en la nube

Se aplica para asegurar los datos que se procesan y almacenan en un entorno de nube. Se usan sistemas de encriptación y de gestión segura de claves para proporcionar integridad y confidencialidad a los datos. 

### Borrado criptográfico

Es un método para borrar la clave de encriptación de los datos encriptados. Es una técnica reciente más eficaz que los métodos tradicionales ya que de esta manera los datos son indescifrables e impide que nadie pueda desencriptarlos. 

### Gestión de claves

La encriptación moderna se basa en mantener seguras las claves de encriptación. A continuación trataremos algunas medidas:

- **Módulo de plataforma de confianza (TPM):** El TPM es un chip de un ordenador que puede almacenar de forma segura contraseñas, certificados y claves de encriptación

- **Módulo de seguridad de hardware de la nube (CloudHSM):** El CloudHSM es un dispositivo informático que proporciona almacenamiento seguro para claves criptográficas y procesa operaciones criptográficas.