# Añadir y eliminar usuarios

Este tema está relacionado con la autenticación. La autenticación es el proceso mediante el cual un usuario demuestra que es quien dice ser en el sistema. Además de todo esto, es muy importante ir añadiendo y eliminado usuarios en función de si entran o salen de la organización. Hay que destacar un tipo de usuario, que es el administrador (root).

- **Root:** Es un usuario con privilegios elevados para modificar el sistema. Los usuarios habituales tienen limitaciones, este no ya que puede crear, eliminar, modificar y ejecutar cualquier archivo o programa. Además, solo los usuarios root pueden añadir nuevos usuarios con comandos pero tenemos que tener mucha precaución ya que no es una buena práctica usar estos comandos en Linux porqué podemos hacer cambios irreversibles. 

Una vez visto el usuario root hemos visto que puede darnos problemas si no lo usamos bien o nos equivocamos. Es por ello que aparece otro comando que es el de 'sudo'. 

- **Sudo:** Es un comando que otorga permisos elevados temporalmente a usuarios específicos y permite ejecutar comandos como usuario avanzado sin tener que cambiar de cuenta. Esto proporciona un enfoque más controlado que el root, que ejecuta todos los comandos con privilegios de root. Aún así, no todos los usuarios del sistema pueden ser superusuarios ya que para serlo tiene que estar definido el usuario en el archivo 'sudoers'. Es importante destacar que no se tiene que usar 'sudo' para todo y solo cuando sea necesario porqué es ir importante ir haciendo todos los protocolos de seguridad y no ir saltandolos con este comando.
<br>

### Autenticación y autorización de sudo

Los comandos clave utilizados para estas tareas son los siguientes: 

- **useradd:** Añade un usuario al sistema. Para añadir un usario con el nombre 'fgarcia' con sudo tendriamos que introducir el siguiente comando: 'sudo useradd fgarcia'. Existen opciones adicionales que podemos utilizar con useradd:

    - **'-g':** Establece el grupo por defecto del usuario, también llamado su grupo primario --> sudo useradd -g security fgarcia
    - **'-G'::** Añade el usuario a grupos adicionales, también llamados grupos suplementarios o secundarios --> sudo useradd -G finance,admin fgarcia

- **usermod:**  Modifica las cuentas de usuarios existentes. También existen opciones adicionales, que son:

    - **'-g':** Para cambiar el grupo primario de un usuario existente --> sudo usermod -g executive fgarcia
    - **'-G':** Para añadir un grupo suplementario para un usuario existente --> sudo usermod -a -G marketing fgarcia

- **userdel:** Elimina un usuario del sistema --> 'sudo userdel fgarcia'. Este comando borraria el usuario 'fgarcia' pero no sus archivos. Si quisiéramos borrar el usuario y también sus archivos tendríamos que usar -r de la siguiente manera --> sudo userdel -r fgarcia

- **chown:** Cambia la propiedad de un archivo o directorio. Podemos utilizar este comando para cambiar la propiedad del usuario o del grupo. Para cambiar el usuario propietario del archivo 'acces.txt' a 'fgarcia' usaríamos --> sudo chown fgarcia access.txt y para cambiar el propietario del grupo de 'acces.txt' a 'security' usaríamos --> sudo chown :security access.txt

