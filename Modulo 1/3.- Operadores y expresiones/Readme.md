# Operadores y expresiones

En este módulo, los estudiantes profundizarán en los operadores y expresiones en Swift. A continuación, se explican los temas principales que se tratarán en este módulo:

## Operadores aritméticos

En este tema, los estudiantes aprenderán acerca de los diferentes operadores aritméticos en Swift, incluyendo la suma, la resta, la multiplicación y la división. Se les mostrará cómo utilizar estos operadores para realizar cálculos simples y complejos en Swift.

```swift
// Suma
var resultado = 5 + 2
print(resultado) // Imprime 7

// Resta
resultado = 10 - 4
print(resultado) // Imprime 6

// Multiplicación
resultado = 3 * 4
print(resultado) // Imprime 12

// División
resultado = 20 / 5
print(resultado) // Imprime 4

// Módulo
resultado = 10 % 3
print(resultado) // Imprime 1
```

## Operadores de comparación

En este tema, los estudiantes aprenderán sobre los operadores de comparación en Swift, que se utilizan para comparar dos valores. Se les mostrará cómo utilizar los operadores de comparación para evaluar si dos valores son iguales, diferentes, mayores o menores que otro.

```swift
// Igual a
var comparacion = 5 == 5
print(comparacion) // Imprime true

// Diferente a
comparacion = 4 != 3
print(comparacion) // Imprime true

// Mayor que
comparacion = 7 > 3
print(comparacion) // Imprime true

// Menor que
comparacion = 2 < 5
print(comparacion) // Imprime true

// Mayor o igual que
comparacion = 5 >= 5
print(comparacion) // Imprime true

// Menor o igual que
comparacion = 7 <= 5
print(comparacion) // Imprime false
```

## Operadores de asignación

En este tema, los estudiantes aprenderán acerca de los operadores de asignación en Swift, que se utilizan para asignar un valor a una variable o constante. Se les mostrará cómo utilizar estos operadores para asignar valores y modificar el valor de una variable o constante.

```swift
// Asignación simple
var miVariable = 10
print(miVariable) // Imprime 10

// Asignación con operación
miVariable += 5
print(miVariable) // Imprime 15

// Asignación con operación de resta
miVariable -= 3
print(miVariable) // Imprime 12
```

## Operadores lógicos

En este tema, los estudiantes aprenderán sobre los operadores lógicos en Swift, que se utilizan para evaluar expresiones booleanas. Se les mostrará cómo utilizar los operadores lógicos para combinar expresiones booleanas y crear expresiones más complejas.

```swift
// AND lógico
var logica = true && false
print(logica) // Imprime false

// OR lógico
logica = true || false
print(logica) // Imprime true

// Negación lógica
logica = !true
print(logica) // Imprime false
```


## Expresiones en Swift

En este tema, los estudiantes aprenderán a utilizar expresiones para crear operaciones más complejas en Swift. Se les mostrará cómo combinar operadores y valores para crear expresiones que realicen cálculos más complejos.

```swift
// Ejemplo de expresión
var resultado = (10 + 5) * 2 / 3
print(resultado) // Imprime 10
```

En general, este módulo proporcionará a los estudiantes una comprensión sólida de los diferentes tipos de operadores y expresiones en Swift. Al final de este módulo, los estudiantes tendrán las habilidades necesarias para utilizar operadores aritméticos, de comparación, de asignación y lógicos para realizar operaciones en Swift, y también sabrán cómo utilizar expresiones para crear operaciones más complejas.


## Ejercicio: Calculadora de propinas

Cree un programa Swift que calcule el costo total de una comida, incluidos los impuestos y la propina. El programa debe solicitar al usuario el costo de la comida, la tasa impositiva y la tasa de propina, luego calcular y mostrar el costo total de la comida.

Aquí un ejemplo de cómo debería funcionar el programa:

```swift
Enter the cost of the meal: 50
Enter the tax rate: 8
Enter the tip rate: 20
The total cost of the meal is $63.20
```

Para completar este ejercicio, necesitará usar variables y constantes para almacenar la entrada del usuario y los valores calculados, operadores aritméticos para realizar los cálculos y expresiones para combinar los valores y operadores.

Aquí hay un código de inicio para ayudarlo a comenzar:

```swift
print("Enter the cost of the meal:")
// Use the readLine() function to read the user's input
// Store the cost of the meal, tax rate, and tip rate in variables or constants
// Use arithmetic operators to calculate the tax and tip amounts
// Use expressions to combine the values and operators
// Display the total cost of the meal using string interpolation
```

¡Buena suerte y diviertete!
