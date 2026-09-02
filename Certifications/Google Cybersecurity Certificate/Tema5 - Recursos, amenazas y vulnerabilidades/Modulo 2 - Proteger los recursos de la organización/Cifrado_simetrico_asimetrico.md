# Cifrado simétrico y asimétrico

- **Simétrico:** Consiste en utilizar una única clave secreta para intercambiar información. Como utiliza una sola clave para cifrar y descifrar, el emisor y receptor deben conocer la clave secreta para bloquear o desbloquear el cifrado.

- **Asimétrico:** Es el uso de un par de claves públicas y privadas para cifrar y descifrar datos. La clave pública se utiliza para cifrar los datos y la privada para descifrarlos. La clave privada sólo se entrega a los usuarios con acceso autorizado.

Los cifradores son vulnerables a los *ataques de fuerza bruta*, que utilizan un proceso de ensayo y error para descubrir información privada. En el cifrado moderno, las longitudes de la clave más largas se consideran más seguras ya que son más dificiles de descubrir con este tipo de ataques. Esto también tiene un inconveniente y es que los tiempos de procesamiento son mas lentos. Por eso hay que buscar un equilibrio entre rapidez y seguridad.
<br>

## Algoritmos aprobados

### Algoritmos simétricos

- **Triple DES (3DES):** Se conoce como algoritmo de cifrado por bloques por la forma en que convierte el texto plano en texto cifrado en "bloques" Sus orígenes se remontan al Data Encryption Standard (DES), desarrollado a principios de la década de 1970. DES fue uno de los primeros algoritmos de encriptación simétrica que generaba claves de 64 bits, aunque sólo se utilizan 56 bits para la encriptación. Un bit es la unidad más pequeña de medida de datos en un ordenador. Como se puede imaginar, Triple DES genera claves tres veces más largas. Triple DES aplica el algoritmo DES tres veces, utilizando tres claves diferentes de 56 bits. El resultado es una longitud de la clave efectiva de 168 bits. A pesar de que las claves son más largas, muchas organizaciones están dejando de utilizar Triple DES debido a las limitaciones en la cantidad de datos que pueden cifrarse. Sin embargo, es probable que Triple DES siga utilizándose por motivos de retrocompatibilidad.

- **Estándar de encriptación avanzada (AES):** Es uno de los algoritmos simétricos más seguros de la actualidad. AES genera claves de 128, 192 o 256 bits. Se considera que las claves criptográficas de este tamaño están a salvo de ataques de fuerza bruta. Se calcula que forzar una clave AES de 128 bits podría llevarle a un ordenador moderno miles de millones de años.
<br>

### Algoritmos asimétricos

- **Rivest Shamir Adleman (RSA):** RSA es uno de los primeros algoritmos de criptografía asimétrica que produce un par de claves pública y privada. Los algoritmos asimétricos como RSA producen longitudes de la clave aún más largas. En parte, esto se debe al hecho de que estas funciones crean dos claves. Los tamaños de la clave RSA son de 1.024, 2.048 o 4.096 bits. RSA se utiliza principalmente para proteger datos muy sensibles.

- **Algoritmo de firma digital (DSA):** Es un algoritmo asimétrico estándar que introdujo el NIST a principios de la década de 1990. DSA también genera longitudes de la clave de 2.048 bits. Este algoritmo se utiliza mucho hoy en día como complemento de RSA en infraestructuras de clave pública.
<br>

### Generación de claves

Estos algoritmos deben implementarse cuando una organización elige uno para proteger sus datos. Una forma de hacerlo es utilizando OpenSSL, que es una herramienta de línea de comandos de código abierto que puede utilizarse para generar claves públicas y privadas. OpenSSL se utiliza habitualmente en ordenadores para verificar certificados digitales que se intercambian como parte de la infraestructura de clave pública.