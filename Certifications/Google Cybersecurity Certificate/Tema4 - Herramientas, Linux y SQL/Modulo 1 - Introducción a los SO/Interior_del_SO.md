# El interior de un SO

El trabajo de un SO es ayudar a que otros programas del ordenador funcionen eficientemente. El procedimiento que sigue es el siguiente:

- Se presiona el botón de encendido, se arranca el ordenador y se instala el SO. Arrancar el ordenador significa que se activa un microchip llamado BIOS, o los mas nuevos que se llaman UEFI, para inicializar el hardware. Tanto la BIOS como la UEFI contienen instrucciones de arranque que son los responsables de cargar un programa especial llamado cargador de arranque (bootloader).

- El bootloader es el responsable de iniciar el SO.

Algunas vulnerabilidades pueden ocurrir durante este proceso ya que a menudo, la BIOS no es explorada por el antivirus i puede ser infectada por un software malicioso.

Ahora veremos como los usuarios se comunica con el sistema para completar tareas:

- Usamos aplicaciones que envian una solicitud al SO.

- El SO interpreta esa solicitud y la dirige al componente de hardware del dispositivo. 

- El hardware enviará información de vuelta al SO.

- Finalmente, esta información se enviará a la aplicación.