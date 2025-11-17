# Ataques de fuerza bruta

Es un ataque que se basa en un proceso de ensayo y error para descubrir información privada. Existen diferentes tipos de ataques de fuerza bruta que los atacantes utilizan para adivinar contraseñas, como:

- **Ataques de fuerza bruta simples:** Cuando los atacantes intentan adivinar las credenciales de inicio de sesión de un usuario, se considera un ataque simple. 

- **Ataques de diccionario:** Los atacantes utilizan una lista de contraseñas de uso común y credenciales robadas en violaciones anteriores para acceder a un sistema. 

Usar fuerza bruta puede ser un proceso tedioso y lento, sobretodo cuando se hace manualmente. Por eso existen herramientas que automatizan estas tareas y llevar a cabo estos ataques más rápido. 
<br>

### Evaluar las vulnerabilidades

Antes de que se produzca un ataque de fuerza bruta o un incidente, las empresas pueden realizar pruebas en su red o aplicaciones para evaluar las vulnerabilidades. Los analistas usan máquinas virtuales o sandbox para probar archivos sospechosos, comprobar vulnerabilidades o simular un incidente de ciberseguridad.

- **Máquinas virtuales (VM):** Proporcionan una capa adicional de seguridad para una organización porque pueden utilizarse para ejecutar código en un entorno aislado, evitando que el código malicioso afecte al resto del ordenador o sistema. Al terminar pueden eliminarse o sustituirse. Muy útiles cuando se investigan máquines infectadas.

- **Sandbox:** Es un entorno de pruebas que permite ejecutar software separado de la red. Suelen utilizarse para probar parches, identificar y solucionar errores o detectar vulnerabilidades de seguridad. Los sandbox también pueden utilizarse para evaluar software sospechoso, evaluar archivos maliciosos y simular escenarios de ataque. 

Aún usando estas herramientas hay que ir con cuidado porqué los atacantes pueden programar su software malicioso para que se comporte como software inofensivo cuando se ejecuta dentro de este tipo de entornos de pruebas.
<br>

### Medidas de prevención

- **Salting y hash:** El hash convierte la información en un valor único que puede utilizarse para determinar su integridad. Es una función unidireccional, lo que significa que es imposible desencriptar y obtener el texto original. El salting añade caracteres aleatorios a las contraseñas hash lo que aumenta la longitud y la complejidad de dichos valores haciéndolos más seguros.

- **Autenticación de múltiples factores (MFA) y autenticación de dos factores (2FA):** MFA es una medida de seguridad que requiere que un usuario verifique su identidad de dos o más formas para acceder a un sistema o una red. La 2FA es similar salvo que solo utiliza dos formas de verificación. 

- **CAPTCHA y reCAPTCHA:** Son las siglas de Completely Automated Public Turing test to tell Computers and Humans Apart (Prueba de Turing pública completamente automatizada para distinguir entre ordenadores y humanos). Pide a los usuarios que completen una sencilla prueba que demuestra que son humanos. Esto ayuda a evitar que el software intente forzar una contraseña. reCAPTCHA es un servicio CAPTCHA gratuito de Google que ayuda a proteger a los sitios web de bots. 

- **Políticas de contraseñas:** Se usan para estandarizar las buenas prácticas de contraseñas en toda la empresa. Las políticas pueden incluir directrices sobre la complejidad de la contraseña, la frecuencia con la que se debe actualizar, si se puede reutilizar o no y si hay límites en el número de veces que un usuario puede intentar iniciar sesión antes de que se suspenda su cuenta.