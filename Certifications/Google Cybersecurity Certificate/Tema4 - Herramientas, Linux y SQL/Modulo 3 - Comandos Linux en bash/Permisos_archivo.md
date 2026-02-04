# Comandos de permiso

### Permisos de lectura

Los permisos se representan con una cadena de 10 caraceteres que incluyen:

- **Leer:** Para archivos, esta es la capacidad de leer el contenido del archivo y para directorios, esta es la capacidad de listar el contenido del directorio incluyendo tanto archivos como subdirectorios. 
- **Escribir:** Para archivos, esta es la capacidad de modificar el contenido del archivo y para directorios, esta es la capacidad de crear nuevos archivos en el directorio. 
- **Ejecutar:** Para archivos, esta es la capacidad de ejecutar el archivo si se trata de un programa y para los directorios, es la capacidad de entrar al directorio y acceder a sus archivos. 

Estos permisos se dan a estos tipos de propietarios:

- **Usuario (u):** El propietario del archivo.
- **Grupo (g):** Un grupo mayor del que forma parte el propietario.
- **Otro (o):** Todos los demás usuarios del sistema.

Cada carácter de la cadena de 10 caracteres (drwxrwxrwx) transmite información diferente sobre los permisos.

- **Carácter 1:** Tipo de archivo: 'd' para directorios y '-' para un archivo.
- **Carácter 2:** Permisos de lectura para el usuario: 'r' si el usuario tiene permisos de lectura y '-' si no.
- **Carácter 3:** Permisos de escritura para el usuario: 'w' si el usuario tiene permisos de escritura y '-' si no.
- **Carácter 4:** Permisos de ejecución para el usuario: 'x' si el usuario tiene permisos de ejecución y '-' si no.
- **Carácter 5:** Permisos de lectura para el grupo: 'r' si el grupo tiene permisos de lectura y '-' si no.
- **Carácter 6:** Permisos de escritura para el grupo: 'w' si el grupo tiene permisos de escritura y '-' si no.
- **Carácter 7:** Permisos de ejecución para el grupo: 'x' si el grupo tiene permisos de ejecución y '-' si no.
- **Carácter 8:** Permisos de lectura para otros: 'r' si los otros tienen permisos de lectura y '-' si no.
- **Carácter 9:** Permisos de escritura para otros: 'w' si los otros tienen permisos de escritura y '-' si no.
- **Carácter 10:** Permisos de ejecución para otros: 'x' si los otros tienen permisos de ejecución y '-' si no.
<br>

### Exploración de los permisos existentes

Podemos utilizar el comando 'ls' para investigar quién tiene permisos sobre archivos y directorios. Para ello existen opciones adicionales que podemos añadir a este comando para que sea más específico y que nos proporcione más detalles sobre los permisos. 

- **ls -a** Muestra los archivos ocultos. Estos archivos comienzan con un punto (.) al principio.
- **ls -l** Muestra los permisos de archivos y directorios. También muestra información adicional, como el nombre del propietario, el grupo, el tamaño del archivo y la hora de la última modificación.
- **ls -la** Muestra los permisos de archivos y directorios, incluidos los ocultos. Es una combinación de las otras dos opciones. 
<br>

### Cambio de permisos

El *principio del privilegio mínimo* es el concepto de conceder sólo el acceso y la autorización mínimos necesarios para completar una tarea o función, porqué los usuarios no deben tener privilegios que vayan más allá de lo necesario. No seguir este principio podria crear riesgos de seguridad. 

El comando 'chmod' nos puede ayudar a gestionar esta autorización porqué cambia los permisos de archivos y directorios.

**chmod:**  Este comando requiere de dos argumentos. El primer argumento indica cómo cambiar los permisos y el segundo argumento indica el archivo o directorio para el que se desea cambiar los permisos. 

Ejemplo:

'chmod u+rwx,g+rwx,o+rwx login_sessions.txt' --> Añadimos todos los permisos al archivo login_sessions.txt.

'chmod u-rwx,g-rwx,o-rwx login_sessions.txt' --> Quitamos todos los permisos al archivo login_sessions.txt.

Este comando sobreescribe los permisos existentes.