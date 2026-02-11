# Filtros básicos en consultas SQL

Filtrar es seleccionar datos que cumplan una determinada condición. Para entenderlo mejor es una manera de elegir los datos que deseamos. 

Antes de seguir con el filtrado tenemos que aclarar un concepto, los operadores.

- **Operadores:** Es un símbolo o palabra clave que representa una operación. Un ejemplo podria ser el operador igual a (=).

Una vez visto esto, para filtrar una consulta SQL tenemos que añadir una línea adicional después del SELECT y el FROM que será la cláusula WHERE. 

- **WHERE:** Es la cláusula que indica la condición para un filtro. Después de esta palabra clave se enumera la condición específica mediante operadores. Ejemplo: WHERE country = 'USA'.

Podemos hacer que nuestras condiciones sean más complejas buscando un patrón en vez de palabras exactas. Para buscar patrones usaremos el símobolo '%' para que actúe como comodín para caracteres no especificados. Ejemplo 'Este%', nos devolvería todos ños registros que comiencen con 'Este'.

Si usamos el símbolo % para buscar patrones, no podremos usar el símbolo =. Es por ello que aparece otra cláusula que es la de LIKE.

- **LIKE:** Es un operador que se utiliza con WHERE para buscar un patrón en una columna. Como es similar al símbolo =, lo usaremos en su lugar. Ejemplo: WHERE office LIKE 'Este%'.

Otro símbolo importante a destacar es el de '_' que sirve para sustituir sólo a otro carácter. 
<br>

### Filtrar fechas y números

En las BD encontraremos prinicpalmente: cadenas, números y fechas. Para poder filtrar los números y las fechas, los operadores más comunes son: =, >, <, !=, >=, <=. Existe otro operador que es el de BETWEEN.

- **BETWEEN:** Es un operador que filtra números o fechas dentro de un rango. Ejemplo: WHERE OS_patch_date BETWEEN '20221-03-01 AND '2021-09-01';.

Es importante destacar que el formato de las fechas es 'AAAA-MM-DD' y el de las horas es 'HH:MM:SS'.
<br>

### Filtrados con AND, OR y NOT

Al hacer consultas tendremos que usar más de una condición muchas veces. Es por ello que existen los siguientes operadores:

- **AND:** Es un operador que especifica que ambas condiciones deben cumplirse a la vez. Ejemplo: WHERE supportrepid = 5 AND country = 'USA';
- **OR:** Es un operador que especifica que al menos una de las condiciones debe cumplirse. Ejemplo: WHERE country = 'Canada' OR country = 'USA';
- **NOT:** Es un operador que especifica que la condición no debe cumplirse. Ejemplo: WHERE NOT country = 'USA';