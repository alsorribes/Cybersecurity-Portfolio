# Tecnología de virtualización

### Máquinas virtuales

Una máquina virtual es una versión virtual de una ordenador físico. La virtualización es el proceso de utilizar software para crear representaciones virtuales de varias máquinas físicas. El término "virtual" se refiere a máquinas que no existen físicamente, pero que funcionan como si lo hicieran porqué su software simula el hardware físico. Los sistemas virtuales no utilizan hardware físico dedicado ya que en su lugar, utilizan versiones definidas por software del hardware físico. Esto significa que una sola máquina virtual tiene una CPU virtual, almacenamiento virtual y otro hardware virtual. 

Se pueden ejecutar varias máquinas virtuales utilizando el hardware físico de un solo dispositivo lo que implica que se tienen que dividir los recursos del dispositivo anfitrión para compartirlos entre todos los componentes físicos y virtuales.
<br>

### Beneficios de las máquinas virtuales

La virtualización puede aumentar la seguridad de muchas tareas y aumentar la eficacia.

- **Seguridad:** Puede proporcionar un entorno aislado con un sandbox en la máquina anfitriona física. Estas máquinas estan aisladas de la máquina host y de otras máquinas virtuales invitadas lo que proporciona una capa de seguridad extra porqué se mantienen separadas de los demás sistemas. En estos sitios es dónde se puede probar software malicioso para examinarlo en un entorno seguro.

- **Eficiencia:** Podemos abrir varias máquinas virtuales y cambiar fácilmente de una a otra lo que permite agilizar tareas de seguridad como probar y explorar varias aplicaciones. 
<br>

### Gestionar máquinas virtuales 

Se pueden gestionar con un software denominado hipervisor que ayudan a conectar el hardware virtual y el físico. Los hipervisores también ayudan a asignar los recursos compartidos de la máquina anfitriona física a una o más máquinas virtuales. 

Un hipervisor conocido es la máquina virtual basada en kernel (KVM). KVM es un hipervisor de código abierto compatible con la mayoría de las principales distribuciones de Linux. Está integrado en el kernel de Linux, lo que significa que puede utilizarse para crear máquinas virtuales en cualquier máquina que ejcute un sistema operativo Linux sin necesidad de software adicional. 