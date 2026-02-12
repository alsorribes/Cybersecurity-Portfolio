# Funciones de agregación en SQL

Son funciones que realizan un cálculo sobre varios puntos de datos y devuelven el resultado de este. Existen varias funciones de agregación, como por ejemplo: 

- **COUNT:** Devuelve un único número que representa el número de filas devueltas por la consulta.

- **AVG:** Devuelve un único número que representa la media de los datos númericos de una columna.

- **SUM:** Devuelve un único número que representa la suma de los datos numéricos de una columna. 

Para usar estas funciones de agregación, tenemos que colocar la palabra correspondiente después de la palabra clave SELECT y, a continuación, poner entre paréntesis el nombre de la columna sobre la que se desea realizar el cálculo.

*Ejemplo:* SELECT COUNT(firstname)
FROM customers;

En este caso nos hará el recuento de esa columna y nos dará el resultado con un valor numérico. 