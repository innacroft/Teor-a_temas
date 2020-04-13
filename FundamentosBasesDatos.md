#Bases de datos relacionales
Una base de datos relacional es un tipo de base de datos que almacena y proporciona acceso a puntos de datos relacionados entre sí. Las bases de datos relacionales se basan en el modelo relacional: una forma intuitiva y directa de representar datos en tablas. 

- Support Standard Markdown / CommonMark and GFM(GitHub Flavored Markdown);

##Conceptos 
- Entidad: Una entidad es un objeto, es la representación de algo en el mundo real.
######Ej: Computadora 💻

- Atributo: conjunto de características que tiene una entidad.
######Ej: Para la entidad  computadora 💻, los atributos pueden ser:
###### - Color 
###### - Año
###### - Modelo
###### - Disco duro
###### - Número de serie
- Relación: Manera en que se vinculan las entidades y están definidas por verbos, por ejemplo
######Ej: Computadora 💻 TIENE Disco duro💽

##Tipos de atributos llave
- Atributos llave naturales: es el atributo ihnerente al objeto, esto quiere decir que es propio del objeto, como un identificador.
######Ej: número de serie, isbn en libros.
- Atributos de llave artificiales: no son inherentes , no son naturales del objeto, son propiedades que se le asignan.
######Ej: al asignar un contador incremental a una lista de objetos y usarlos como identificador único.
##Tipos de entidades
- Entidades débiles: no pueden existir sin las entidades fuertes.
	- Entidades débiles por identidad: no pueden existir sin las entidades fuertes.
	- Entidades débiles por existencia: asigna clave propia pero va a depender de la fuerte.
- Entidades fuertes: son entidades que existen por si solas.
##Tipos de relaciones entre entidades
- Uno a uno (1:1) :
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)
- Cero a uno (0:1) :
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)
- Uno a muchos (1:n) :
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)
- Cero a muchos (0:n) :
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)
- Muchos a muchos (n:n) :
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)
##Diagrama entidad relacion
![](https://pandao.github.io/editor.md/images/logos/editormd-logo-180x180.png)



##Tipos de datos:

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


