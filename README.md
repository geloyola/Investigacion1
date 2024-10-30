# Investigacion1
Trabajo de investigacion de Programacion funcional y reactiva

## Que son las funciones sin nombres?
Una función sin nombre o anónima es un bloque de código que se define de forma directa, sin asignarle un nombre, y generalmente se utiliza en contextos donde una función solo se necesita una vez o se quiere mantener el código breve y claro.

### Definicion de Funciones Anónimas
Una función anónima en Scala es una función que no tiene un nombre y se define usando el símbolo =>. En la parte izquierda del => van los parámetros, y en la parte derecha va el código que queremos ejecutar con esos parámetros.

Una función anónima en Scala es una función que no tiene un nombre y se define usando el símbolo =>. En la parte izquierda del => van los parámetros, y en la parte derecha va el código que queremos ejecutar con esos parámetros.
// Definimos una función anónima que suma dos números
val suma: (Int, Int) => Int = (a: Int, b: Int) => { a + b }

En esta función:

- (a: Int, b: Int) son los parámetros de tipo Int.
- a + b es lo que hace la función, que en este caso suma a y b.
  
Para usar esta función anónima, simplemente llamamos a suma y le pasamos los números:
// Llamada a la función anónima a través de la variable suma
val resultado = suma(6, 4)
println(s"El resultado de la suma es " + resultado)
Al ejecutar esto veremos que se va a mostrar el resultado de la suma que es: 10

### Funciones Lambda
Son funciones anonimas que se definen en el lugar donde se necesitan. Estas funciones se utilizan para crear bloques de código rápidos y compactos, sobre todo cuando necesitamos pasar una función como parámetro a otro método, como map, filter, o reduce.
#### Caracteristicas de la Funcion Lambda
* Sintaxis Concisa: En Scala, las funciones lambda se definen con la sintaxis (parametros) => cuerpo.
* Uso en Funciones de Orden Superior: Las lambdas son muy útiles en funciones de orden superior que necesitan recibir otras funciones como argumentos.
* Flexibilidad: Son ideales para definir funciones temporales y simplificar el código, ya que no requieren de una declaración por separado.

### Funcion con Nombre a Funcion sin Nombre

#### Funcion con Nombre: 

def f(n: Int) = (1 to n).product

Esta función f calcula el producto de todos los números de 1 a n (equivalente al factorial de n). 
Para cambiar esta funcion a una funcion sin nombre o anonima lo hacemos asi:

val producto = (n: Int) => (1 to n).product

(n: Int) => representa los parámetros de entrada de la función
(1 to n).product es el cuerpo de la función, que calcula el producto de los números de 1 a n.


Bibliografia: 
https://keepcoding.io/blog/funciones-anonimas-en-javascript/#:~:text=Las%20funciones%20an%C3%B3nimas%20en%20JavaScript%20son%20aquellas%20que%20no%20han,los%20modos%20de%20escribir%20funciones.
https://www.arteco-consulting.com/articulos/introduccion-java-lambda/#:~:text=Las%20funciones%20lambdas%20es%20un,o%20ning%C3%BAn%20valor%20de%20retorno.


