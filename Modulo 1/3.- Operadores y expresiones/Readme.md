# Operadores y expresiones

Swift proporciona un amplio conjunto de operadores que se pueden usar para realizar varias operaciones en los datos. En esta sección, profundizaremos en los operadores y expresiones de Swift y aprenderemos a usarlos para crear operaciones más complejas.

## Operadores aritméticos

Los operadores aritméticos se utilizan para realizar operaciones aritméticas básicas con datos numéricos. Swift proporciona los siguientes operadores aritméticos:

- Suma: `+`
- Resta: `-`
- Multiplicacion: `*`
- Divicion: `/`
- Modulo: `%`

Estos son algunos ejemplos del uso de operadores aritméticos en Swift:

```swift
let sum = 10 + 5 // Addition
let difference = 10 - 5 // Subtraction
let product = 10 * 5 // Multiplication
let quotient = 10 / 5 // Division
let remainder = 10 % 3 // Remainder
```

## Operadores de comparación

Los operadores de comparación se utilizan para comparar dos valores y devolver un valor booleano (verdadero o falso). Swift proporciona los siguientes operadores de comparación:

- Igual a: `==`
- Diferente a: `!=`
- Mayor que: `>`
- Menor que: `<`
- Mayor o igual que: `>=`
- Menor o igual que: `<=`

Estos son algunos ejemplos del uso de operadores de comparación en Swift:

```swift
let isGreaterThan = 10 > 5 // Greater than
let isLessThan = 10 < 5 // Less than
let isEqual = 10 == 5 // Equal to
let isNotEqual = 10 != 5 // Not equal to
```

## Operadores de asignación

Los operadores de asignación se utilizan para asignar un valor a una variable o constante. Swift proporciona varios operadores de asignación, que incluyen:

- Asignación sencilla: `=`
- Asignación de adición: `+=`
- Asignación de resta: `-=`
- Asignación de multiplicación: `*=`
- Asignación de división: `/=`
- Asignación Modulo: `%=`

Estos son algunos ejemplos del uso de operadores de asignación en Swift

```swift
var score = 0 // Simple assignment
score += 10 // Addition assignment
score -= 5 // Subtraction assignment
score *= 2 // Multiplication assignment
score /= 3 // Division assignment
score %= 2 // Remainder assignment
```

## Operadores logicos

Los operadores lógicos se utilizan para combinar valores booleanos y devolver un resultado booleano. Swift proporciona los siguientes operadores lógicos:

- Logical NOT: `!`
- Logical AND: `&&`
- Logical OR: `||`

Estos son algunos ejemplos del uso de operadores lógicos en Swift:

```swift
let isTrue = true && false // Logical AND
let isFalse = true || false // Logical OR
let isNot = !true // Logical NOT
```

## Expresiones

Las expresiones son combinaciones de valores, variables, operadores y llamadas a funciones que dan como resultado un solo valor. Swift proporciona un sistema de expresiones potente y flexible que le permite crear operaciones complejas mediante una combinación de operadores y expresiones. Estos son algunos ejemplos del uso de expresiones en Swift:

```swift
let result = (10 + 5) * 2 // Evaluates to 30
let isInRange = (1...10).contains(5) // Evaluates to true
let message = "Hello, " + "World!" // Evaluates to "Hello, World!"
```

Al dominar los operadores y las expresiones en Swift, podrá escribir programas más complejos y potentes.

## Ejercicio: Calculadora de propinas

Cree un programa Swift que calcule el costo total de una comida, incluidos los impuestos y la propina. El programa debe solicitar al usuario el costo de la comida, la tasa impositiva y la tasa de propina, luego calcular y mostrar el costo total de la comida.

He aquí un ejemplo de cómo debería funcionar el programa:

```
Enter the cost of the meal: 50
Enter the tax rate: 8
Enter the tip rate: 20
The total cost of the meal is $63.20
```

Para completar este ejercicio, necesitará usar variables y constantes para almacenar la entrada del usuario y los valores calculados, operadores aritméticos para realizar los cálculos y expresiones para combinar los valores y operadores.

Aquí hay un código de inicio para ayudarlo a comenzar:

```
print("Enter the cost of the meal:")
// Use the readLine() function to read the user's input
// Store the cost of the meal, tax rate, and tip rate in variables or constants
// Use arithmetic operators to calculate the tax and tip amounts
// Use expressions to combine the values and operators
// Display the total cost of the meal using string interpolation
```

¡Buena suerte y diviertete!
