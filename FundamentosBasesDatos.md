# Bases de datos relacionales
Una base de datos relacional es un tipo de base de datos que almacena y proporciona acceso a puntos de datos relacionados entre sí. Las bases de datos relacionales se basan en el modelo relacional: una forma intuitiva y directa de representar datos en tablas. 

- Support Standard Markdown / CommonMark and GFM(GitHub Flavored Markdown);

## Conceptos 
- Entidad: Una entidad es un objeto, es la representación de algo en el mundo real.
###### Ej: Computadora 💻

- Atributo: conjunto de características que tiene una entidad.
###### Ej: Para la entidad  computadora 💻, los atributos pueden ser:
###### - Color 
###### - Año
###### - Modelo
###### - Disco duro
###### - Número de serie
- Relación: Manera en que se vinculan las entidades y están definidas por verbos, por ejemplo
###### Ej: Computadora 💻 TIENE Disco duro💽

## Tipos de atributos llave
- Atributos llave naturales: es el atributo ihnerente al objeto, esto quiere decir que es propio del objeto, como un identificador.
###### Ej: número de serie, isbn en libros.
- Atributos de llave artificiales: no son inherentes , no son naturales del objeto, son propiedades que se le asignan.
###### Ej: al asignar un contador incremental a una lista de objetos y usarlos como identificador único.
## Tipos de entidades
- Entidades débiles: no pueden existir sin las entidades fuertes.
	- Entidades débiles por identidad: no pueden existir sin las entidades fuertes.
	- Entidades débiles por existencia: asigna clave propia pero va a depender de la fuerte.
- Entidades fuertes: son entidades que existen por si solas.
## Tipos de relaciones entre entidades
- Uno a uno (1:1) :
![](https://github.com/innacroft/Teoria_temas/blob/master/images/1_1.PNG)
- Cero a uno (0:1) :
![](https://github.com/innacroft/Teoria_temas/blob/master/images/0_0.PNG)
- Uno a muchos (1:n) :
![](https://github.com/innacroft/Teoria_temas/blob/master/images/1_n.PNG)
- Cero a muchos (0:n) :
![](https://github.com/innacroft/Teoria_temas/blob/master/images/0_n.PNG)
- Muchos a muchos (n:n) :
![](https://github.com/innacroft/Teoria_temas/blob/master/images/n_n.PNG)

## Diagrama entidad relacion (ERD)
![](https://github.com/innacroft/Teoria_temas/blob/master/images/ER.png)


## Tipos de datos:

 TEXTO :
> CHAR --> cadenas alfanuméricas de longitud  fija.
> VARCHAR --> cadenas alfanuméricas de longitud variable.
> TEXT --> cadenas alfanuméricas normalmente muy extensas.

NUMERICOS: 
> INT -->  números enteros con rango desde 	-2^31 (-2,147,483,648) a 2^31-1 (2,147,483,647).
>BIGINT -->  números enteros con rango desde 	-2^63 (-9,223,372,036,854,775,808) a 2^63-1 (9,223,372,036,854,775,807).
>SMALLINT --> números enteros con rango desde -2^15 (-32,768) a  2^15-1 (32,767).
>DECIMAL --> números decimales.
>NUMERIC --> números decimales.

FECHA:
> DATE --> tipo de dato que sirve para agregar dia, mes y año dentro de un mismo dato tiene un rango entre 0001-01-01 y 9999-12-31.
>TIME  -->  define una hora del día basado en el reloj de 24 horas, tiene un rango de 00:00:00.000000 hasta 23:59:59.9999999
>DATETIME  -->  define una fecha combinada con una horas, minutos y segundos, tiene un rango de '1000-01-01 00:00:00' a '9999-12-31 23:59:59'.
>TIMESTAMP  --> es semejante al datetime, pero el rango está definido desde '1970-01-01 00:00:01' UTC hasta  '2038-01-19 03:14:07'

LOGICOS
>BOOLEAN --> Tipo de dato que puede tener sólo dos estados TRUE y FALSE

## Restricciones bases de datos
- NOT NULL : no se aceptan valores nulos.
- UNIQUE : los valores deben ser únicos.
- PRIMARY KEY: la llave primaria debe ser no ser nula y debe ser única.
- FOREIGN KEY: la llave foránea debe no ser nula y debe ser única.
- CHECK: asegura que el valor de una columna cumpla una condición.
- DEFAULT: coloca un valor por defecto si este no tiene un valor especificado.
- INDEX: se crea por columnas para permitir búsquedas rápidas 
Por lo anterior, existe la normalización: 

## Normalización
La normalización es poner una tabla de forma normal, sin datos duplicados ni uniones extrañas.
- FN : Forma normal.
- 1FN : Elimina los datos duplicados,una tabla no puede tener dos campos iguales. 
- 2FN : Además de cumplir la anterior, se cumple que todos los datos de una tabla que no son clave principal sólo dependen de una clave principal. Nunca habrá dos claves principales en una tabla.
- 3FN : Además de cumplir loas dos anteriores, se cumple que: sólo los campos claves tienen dependencias. Una tabla no puede depender de otra por un campo que no sea clave.
- 4FN : Cumple todos los anteriores y además: los campos multi-evaluados tienen una sola clave única.


## Lenguaje de definición de datos (DDL)
Son sentencias que ayudan a  crear  y modificar la estructura de la base de datos.
- CREATE: Crea objetos de la base de datos 
- ALTER (ADD, ALTER): modifica tablas de la base de datos.
- DROP: elimina objetos de la base de datos.
- TRUNCATE: elimina registos de la tabla de la base de datos.

## Lenguaje de manipulaciónde datos (DML)
Es el lenguaje que permite manipular los datos en una base de datos.
- INSERT: inserta o agrega una region en la base de datos.
- UPDATE: permite actualizar o editar datos.
- DELETE: permite eliminar datos.
> ⚠️⚠️⚠️ Se debe tener mucha precaución cuando se utiliza este comando, ya que podría eliminar datos o tablas de manera permanente. 
- SELECT: permite traer información de la base de datos.

## Consultas o Querys

Una vez planteada una buena estructura de la base de datos, y después de haber suministrado datos a la base de datos, las consultas son parte fundamental de las bases de datos, ya que permiten son un tipo de sentencias que permiten extraer los datos y convertirlos en información útil.
De nada sirve tener un montón de registros y no poder hacer nada con ellos. 

La estructura básica de un Query es la siguiente
SELECT dato FROM tabla; 

## Filtros
La estructura básica de un Query traerá toda la información de la columna dato de la tabla, pero necesitaremos aplicar algún tipo de *FILTRO*, para que la información obtenida sea  la que se desea, y también se puede ordenar para que la información se muestre como se desea también. A continuación se muestra como 

## WHERE
Esta es una de las consultas más básicas y permiten traer información dependiendo de la condición dada
###### Ej: tabla números : número del 1 al 40, para cada número hay un nombre de una persona asignado.
###### Deseo traer el nombre de la persona que corresponde al número 3.
###### La sentencia sería:
###### SELECT name FROM NUMEROS WHERE num=3 ;
###### Lo anterior retornaría el nombre de la persona con el numero 3 de la tabla 

### ORDER BY

Este tipo de comandos permiten agrupar objetos , ordenarlos alfabéticamente o numéricamente o agregar algún tipo de filtro.

Teniendo en cuenta este diagrama: 

![](https://github.com/innacroft/Teoria_temas/blob/master/images/user.PNG)

Cuando se necesita traer información de dos o más tablas distintas pero que poseen una relación en el caso anterior de usuario con post , pueden usarsen algunas de las siguientes operaciones:
### JOIN
![](https://github.com/innacroft/Teoria_temas/blob/master/images/conjuntos_.png)

Lo anterior es mucha teoría que puede ser engorrosa, entonces...
## ¿Cómo realizar un Join?
Teniendo en cuenta la siguiente estructura 
![](https://github.com/innacroft/Teoria_temas/blob/master/images/diagrama_transactions.png)
###### Las tablas anteriores corresponden a una base de datos para una librería, la tabla de transacciones corresponden al estado del libro si es ###### prestado o vendido, se desea realizar una consulta que me traiga el nombre del cliente(tabla clients), el titulo del libro(tabla books) y el ###### tipo de transacción(tabla transactions). 

1.Usar como pivote la tabla principal que sería la tabla transactions, es principal porque es de allí donde las demás tablas se relacionan.
2.Relacionar las tablas book y client con transactions, para ello usaremos los *ALIAS*, en este caso son los  *as* y los *on* para unir las tablas,así:<br>
*SELECT* <br>
*FROM TRANSACTIONS AS T* <br>
*JOIN BOOKS AS B* <br>
*ON T.BOOK_ID = B.BOOK_ID* <br>
*JOIN CLIENTS AS C* <br>
*ON T.CLIENT_ID = C.CLIENT_ID* <br>






