# Consultas a las bases de datos con SQL

SQL es un lenguaje de programación utilizado para crear, interactuar y solicitar información en una BD.

- **Consultas:** Una consulta es una solicitud de datos de una tabla de una BD o de una combinación de tablas. 

SQL nos puede ayudar a recuperar registros de un sistema. Antes de seguir vamos a definir lo que es un registro.

- **Registro:** Es una lista de los eventos que se producen en los sistemas de una organización (logs). Estas listas pueden ser enormes pero por eso usamos SQL para poder hacer consultas y encontrar los registros que necesitamos mucho más rápidamente.
<br>

### Consulta SQL básica

Hay dos palabras clave en cualquier consulta SQL: SELECT y FROM.

- **SELECT:** Indica que columnas devolver. Podemos seleccionar varias columnas separándolas por una coma o incluso si queremos obtener todas las columnas de una tabla podemos usar SELECT *.

- **FROM:** Indica que tabla consultar y siempre va después de la palabara clave SELECT. Para finalizar una consulta podemos usar ';' para indicar a SQL que se trata de una consulta completa. 
<br>

### Ordenación

Las tablas de bases de datos suelen ser muy complejas y es por ello que aparecen otras palabras útiles como la de ORDER BY que sirve para organizar los datos que se extraen de una tabla.

- **ORDER BY:** Ordena los registros devueltos por una consulta en función de una o varias columnas especificadas. Pueden ser en orden ascendente o descendente. Se escribe al final de la consulta, justo después del FROM.

    - **Ascendente:** Por defecto se usará este tipo de ordenación al hacer una consulta. 
    - **Descendente:** Para usar este tipo de ordenación tenemos que usar la palabra clave DESC.
    - **Varias columnas:** Podemos hacer una consulta de varias columnas para tener ordenaciones mas específicas. Primero se ordenará la primera columna, luego la segunda y así sucesivamente.