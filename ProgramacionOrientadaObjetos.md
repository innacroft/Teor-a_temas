# PROGRAMACION ORIENTADA A OBJETOS
La programación orientada a objetos es un paradigma* de programación que usa objetos y sus interacciones para la creación de programas informáticos, la programación orientada a objetos busca mantener un código bien estructurado no extenso, modularizado, fácil de leer y de fácil mantenimiento.
**Paradigma: teoría que suministra la base y modelo para resolver problemas.*
## Conceptos 
- Objetos: Un objeto es la abstracción de "algo" en la vida real, el objeto describe principalmente las propiedades(atributos) y el comportamiento(métodos) de ese "algo".También se le conoce como la instancia de una clase.
Los objetos pueden ser físicos o conceptuales.
###### Ej: Persona, Cuenta Bancaria, Perro, Planta, Equipo de fútbol
- Atributos: Un atributo es un sustantivo que se es propio de un objeto, define características de un objeto
###### Ej: OBJETO: Perro | ATRIBUTOS: Nombre, Tamaño, Raza, Sexo, Edad.
- Métodos: Un método define una acción que es del objeto, se representa en un verbo. 
###### Ej: OBJETO: Perro | METODOS: Comer, Dormir,Ladrar,Jugar.

- Clase: una clase se podría definir como el molde u modelo sobre el cual se crea un objeto, gracias a esta se pueden generar múltiples objetos sin necesidad de repetir código.
- Instancia: realización de una clase o propotipo determinado. 

## PRINCIPIOS DE LA PROGRAMACIÓN ORIENTADA A OBJETOS
- Abstracción 👀 : es la capacidad de modelar y extraer las características de "algo" para que este sea un objeto. 
- Encapsulamiento 🌐: esto permite que un dato dentro de una clase sea inalterable, es decir que mantenga cierta seguridad para que no todo el mundo pueda accede a ella para modificarla o verla.
- Modularidad ✂️ : permite dividir la aplicación en partes muy pequeñas, de manera que esto permite que el código sea más legible, se evitan colapsos, sirve para reutilizar código, hace el código mantenible, permite mayor legibilidad y la resolución rápida de problemas.
- Polimorfismo ⭐️ : es la capacidad de los objetos de tomar el mismo nombre pero comportarse de manera diferente.
- Herencia 👪 : permite la reutilización de código, ya que , a partir de la similitud entre objetos se pueden crear clases padres que pueden ser heredadas por sus hijos y así reutilizar el código. 

## Modificadores de acceso
Las variables , métodos y objetos dentro de una clase pueden tener un rango de "seguridad", que permiten que otras clases y su misma clase sean visibles y editables o no. Los modificadores de acceso son esos niveles de seguridad y son los siguientes:
PUBLIC --> Todas las clases tienen acceso.
PROTECTED --> Sólo las clases, paquetes y subclases tienen acceso.
DEFAULT --> las clases y paquetes internos.
PRIVATE --> sólo las clases.

## Representación gráfica
Para representar gráficamente y realizar el modelo de un sistema para posteriormente codificar, es el lenguaje unificado de modelado UML.
La estructura básica para un objeto es un rectángulo de tres secciones así:<br>
![](https://github.com/innacroft/Teoria_temas/blob/master/images/uml1.png)
Se representan teniendo en cuenta los niveles de visibilidad o modificadores de  de los métodos y atributos , los cuales se representan con los siguientes símbolos:
-private
+public
#protected
~default
Este podría ser un ejemplo muy simple: <br>
![](https://github.com/innacroft/Teoria_temas/blob/master/images/uml2.PNG)
Cuando existe más de un objeto, se deben agregar relaciones entre los objetos, es decir entre los recuadros dibujados se debe dibujar una línea pero el final o comienzo de ésta representará algo en específico así:
- AGREGACIÓN: Un elemento dependerá de muchos otros, se representa con un *rombo vacío al final de la línea*.
- COMPOSICIÓN: Un elemento dependerá de muchos otros, pero de manera comprometida, conceptualmente esto significa que una clase no puede vivir sin la otra. Se representa gráficamente como un *rombo relleno al final de la línea*.
- ASOCIACION: este elemento contiene al otro en su definición.Apunta hacia la dependencia y se representa con una flecha sencilla de tres palos así -> .
- HERENCIA: la flecha apunta del hijo al padre, la representación es una flecha triangular vacía.
- DEPENDENCIA: Es una relación de significado entre dos elementos, donde cualquier cambio a un elemento independiente, puede afectar el significado de otro elemento dependiente. Se representa gráficamente como una línea discontinua en trozos y con una flecha sencilla de tres palos.


El siguiente ejemplo es  un ejemplo de un gráfico UML para Un libro de contactos. 
![](https://github.com/innacroft/Teoria_temas/blob/master/images/uml2.gif)




