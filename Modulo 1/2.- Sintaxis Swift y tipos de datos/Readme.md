# Sintaxis Swift y tipos de datos

En este módulo, los estudiantes aprenderán sobre la sintaxis básica y los tipos de datos en Swift. A continuación, se explican los temas principales que se tratarán en este módulo:

## Declaración de variables y constantes

En este tema, los estudiantes aprenderán a declarar variables y constantes en Swift. Se les mostrará cómo declarar una variable utilizando la sintaxis `var`, y cómo declarar una constante utilizando la sintaxis `let`. También se explicará la diferencia entre variables y constantes, y cuándo es apropiado utilizar cada uno.

```swift
// Declaración de una variable
var miVariable = "Hola"
miVariable += " mundo"
print(miVariable) // Imprime "Hola mundo"

// Declaración de una constante
let pi = 3.1416
print(pi) // Imprime 3.1416
```

## Tipos de datos en Swift

En este tema, los estudiantes aprenderán acerca de los diferentes tipos de datos disponibles en Swift. Se les mostrará cómo declarar tipos de datos como cadenas de texto, enteros y números de punto flotante. También se discutirán otros tipos de datos como los booleanos y los arrays.

```swift
// Declaración de una cadena de texto
var miCadena: String = "Esto es una cadena de texto"
print(miCadena) // Imprime "Esto es una cadena de texto"

// Declaración de un entero
var miEntero: Int = 42
print(miEntero) // Imprime 42

// Declaración de un número de punto flotante
var miFlotante: Double = 3.14
print(miFlotante) // Imprime 3.14
```

## Operadores en Swift

En este tema, los estudiantes aprenderán sobre los operadores integrados en Swift. Se les mostrará cómo utilizar los operadores aritméticos, comparativos y lógicos para realizar operaciones en Swift. También se discutirán los operadores de asignación y los operadores de incremento y decremento.

```swift
// Operadores aritméticos
var resultado = 5 + 2
print(resultado) // Imprime 7

resultado = 10 - 4
print(resultado) // Imprime 6

resultado = 3 * 4
print(resultado) // Imprime 12

resultado = 20 / 5
print(resultado) // Imprime 4

// Operadores de comparación
var comparacion = 5 == 5
print(comparacion) // Imprime true

comparacion = 4 < 3
print(comparacion) // Imprime false

comparacion = 7 >= 7
print(comparacion) // Imprime true

// Operadores lógicos
var logica = true && false
print(logica) // Imprime false

logica = true || false
print(logica) // Imprime true
```