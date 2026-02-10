# Introducción a las bases de datos

Una base de dastos es una colección organizada de información o datos. A menudo se comparan con las hojas de cálculo pero estas están más pensadas para un usuario o un equipo pequeño. Las BD pueden almacenar cantidades enormes de datos y pueden ser consultadas simultáneamente por varias personas. Hay muchas bases de datos pero por ahora vamos a tratar las bases de datos relacionales. 

- **BD relacionales:** Es una base de datos estructurada que contiene una o varias tablas que se relacionan entre sí. Estas tablas tienen un conjunto de filas que se llaman registros. Estas filas se rellenan con datos específicos relacionados con la columna de la tabla. Podemos conectar dos tablas si estas dos comparten un columna en común las cuales se denominan claves. 

Una vez visto las BD relacionales y mencionadas las claves hay que distinguir los tipos de claves que hay, que son los siguientes:

- **Clave primaria:** Se refiere a una columna en la que cada fila tiene una entrada única. Esta clave no debe tener valores duplicados, ni valores nulos o vacíos. Además, este tipo de clave nos permite identificar de froma única cada fila de nuestra tabla.

. **Clave foránea:** Es una columna de una tabla que es clave primaria en otra tabla de la BD y estas sí que pueden tener valores duplicados o vacíos. Estas claves nos permiten conectar dos tablas entre sí. Es importante destacar que una tabla solo puede tener una clave primaria y múltiples claves foráneas.

