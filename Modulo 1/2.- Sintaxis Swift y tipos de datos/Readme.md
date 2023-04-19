# Sintaxis Swift y tipos de datos

Swift es un lenguaje de programación de tipo estático, lo que significa que cada variable y constante debe tener un tipo específico. Estos son los tipos de datos básicos en Swift:

## Enteros

Los enteros son números enteros, ya sean positivos o negativos. Están representados por el tipo Int en Swift, que puede tener diferentes tamaños según la plataforma. Aquí hay unos ejemplos:

```swift
let myAge = 30 // A positive integer
let yourAge: Int = -25 // A negative integer
```

## Números de punto flotante

Los números de punto flotante son números con un componente fraccionario, como 3,14 o -2,5. Están representados por los tipos Double y Float en Swift, que tienen diferentes precisiones. Aquí hay unos ejemplos:

```swift
let pi = 3.14159 // A double-precision floating-point number
let e: Float = 2.71828 // A single-precision floating-point number
```

## Strings

Las cadenas son secuencias de caracteres, como "¡Hola, mundo!" o "¡Swift es genial!". Están representados por el tipo String en Swift y se pueden crear usando literales de cadena o concatenando otras cadenas. Aquí hay unos ejemplos:

```swift
let message = "Hello, World!" // A string literal
let name = "John"
let greeting = "Hi, " + name // Concatenating strings
```

## Booleanos

Los booleanos son valores lógicos que pueden ser verdaderos o falsos. Están representados por el tipo Bool en Swift y, a menudo, se usan en declaraciones condicionales y bucles. Aquí hay unos ejemplos:

```swift
let isRaining = true // A true boolean value
let isSunny: Bool = false // A false boolean value
```

## Variables y constantes

Las variables y constantes se utilizan para almacenar valores en Swift. Las variables se declaran con la palabra clave var y sus valores se pueden cambiar a lo largo del programa. Las constantes se declaran con la palabra clave let y sus valores no se pueden cambiar una vez que se asignan. Aquí hay unos ejemplos:

```swift
var score = 0 // A variable that can be changed
score = 10 // The value of the variable is updated

let maxScore = 100 // A constant that cannot be changed
// maxScore = 200 // This would cause a compile-time error
```

## Operadores Swift

Swift tiene muchos operadores integrados que se pueden usar para realizar operaciones aritméticas, de comparación y lógicas en los datos. Aquí hay unos ejemplos:

```swift
// Arithmetic operators
let sum = 10 + 5 // Addition
let difference = 10 - 5 // Subtraction
let product = 10 * 5 // Multiplication
let quotient = 10 / 5 // Division

// Comparison operators
let isGreater = 10 > 5 // Greater than
let isLess = 10 < 5 // Less than
let isEqual = 10 == 5 // Equal to
let isNotEqual = 10 != 5 // Not equal to

// Logical operators
let isTrue = true && false // Logical AND
let isFalse = true || false // Logical OR
let isNot = !true // Logical NOT
```

Al dominar la sintaxis básica y los tipos de datos en Swift, estará bien encaminado para convertirse en un programador de Swift competente.
