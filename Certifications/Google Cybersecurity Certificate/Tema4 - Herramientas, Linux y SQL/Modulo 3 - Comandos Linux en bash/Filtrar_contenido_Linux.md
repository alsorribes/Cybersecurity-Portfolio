# Filtrado de contenidos en Linux

### Filtrar información

Filtrar es seleccionar datos que coincidan con una determinada condición. Nos permite buscar basándonos en criterios específicos, como la extensión de archivo o una cadena de texto.

- **grep:** Busca en un archivo especificado y devuelve todas las líneas del archivo que contengan una cadena o texto especificado. Este comando suele tomar dos argumentos: una cadena que buscar y un archivo en el que buscar --> grep OS updates.txt.
<br>

### Canalización

Para acceder al comando pipe se utiliza el carácter (|). Envía la salida estándar de un comando como entrada estándar a otro comando para su posterior procesamiento. 

Cuando se utiliza con grep, la tubería nos puede ayudar a encontrar directorios y archivos que contengan una palabra específica en sus nombres. Por ejemplo 'ls /home/analyst/reports | grep users' devuelve los nombres de archivos y directorios del directorio 'reports' que contienen 'users'. Antes de la tubería, ls indica que se listen los nombres de los archivos y directorios en 'reports'. Luego, envía esta salida al comando después de la tubería. En este caso, 'grep users' devuelve todos los nombres de archivos y directorios que contienen 'users' de la entrada que recibió. 
<br>

### Buscar

El comando 'find' busca directorios y archivos que cumplan los criterios especificados. Cuando se usa, el primer argumento indica dónde empezar a buscar. Por ejemplo, si se introduce 'find /home/analyst/projects', se buscará todo a partir del directorio 'projects'.

Después de este primer argumento, se tiene que indicar los criterios para la búsqueda para acotar la salida estándar. 

La especificación de criterios implica opciones. Las opciones modifican el comportamiento de un comando y suelen comenzar con un guión. 

- **-nombre y -nombre:** Sirve para encontrar una cadena específica. La cadena que se busca debe introducirse entre comillas después de las opciones '-name' o '-iname'. --> find /home/analyst/projects -name "*log*"

- **-mtime** Sirve para buscar archivos o directorios modificados por última vez en un periodo de tiempo. El número que ponemos en el comando significa el máximo de días de los archivos modificados que queremos ver. --> 'find /home/analyst/projects -mtime -3'