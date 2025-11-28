# Introducción al shell

Es el intérprete de la línea de comandos con lo cual nos ayuda a comunicarnos con el SO. Shell proporciona la interfaz de la línea de comandos para interactuar con él.

Un comando es una instrucción que le dice al ordenador que haga algo para después recibir una respuesta. El shell se comunica con el kernel para ejecutarlos.
<br>

### Tipos de shell

- Bourne-Again Shell (bash).
- C Shell (csh).
- Shell Korn (ksh)
- Shell C mejorada (tcsh).
- Shell Z (zsh).

Todas las shells de Linux utilizan los comandos comunes aunque pueden diferir en otras características. La más popular es bash.
<br>

### Entrada y salida del shell

Los comandos del shell pueden tomar entrada, salida o dar mensajes de error. Vamos a ver la entrada estándar, la salida estándar y los mensajes de error:

- **Entrada estándar:** Consiste en información recibida por el SO a través de la línea de comandos que se introduce desde el teclado. Si el shell puede interpretar la petición, pide al kernel los recursos que necesita para ejecutar esa tarea. 

- **Salida estándar:** Es a información que devuelve el SO a través del shell. Es la respuesta al comando que le hemos introducido anteriormente.

- **Error estándar:** Contiene mensajes de error devueltos por el SO a través del shell en caso de que no tenga una respuesta a nuestro comando. 