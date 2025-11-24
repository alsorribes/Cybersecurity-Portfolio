# Solicitudes al SO

### Iniciar el dispositivo

Cuando encendemos el dispositivo se activa el microchip BIOS (Sistema básico de entrada/salida) o UEFI (Interfaz de Firmware Extensible Unificada). Los dos son microchips que contienen instrucciones para arrancar un dispositivo pero la BIOS es para sistemas antiguos y la UEFI para sistemas más modernos, ya que proporciona mayor seguridad.

La última instruccion FROM de estos microchips activa el bootloader. És un programa que inicia el sistema operativo y, una vez termina, el dispositivo ya está listo para usarse.
<br>

### Finalización de una tarea

Completar una tarea es un proceso que consta de cuatro partes: 

- **Usuario:** Es quién inicia el proceso porqué tiene que realizar algo en el dispositivo. 

- **Aplicación:** És el software con el que interactúan los usuarios para completar una tarea. 

- **Sistema Operativo:** El SO recibe la solicitud del usuario desde la aplicación, tiene que interpretarla, dirigir su flujo y enviarla a los componentes de hardware que correspondan. 

- **Hardware:** És donde se realiza el proceso para completar las tareas necesarias. Una vez hehco el trabajo, devuelve el resultado a través del SO a la aplicación para que esta pueda mostrar los resultados al usuario.