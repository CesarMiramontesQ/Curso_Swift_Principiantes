# Flujo de control y sentencias condicionales

Las declaraciones de flujo de control se utilizan para controlar el flujo de un programa en función de ciertas condiciones. En Swift, existen varios tipos de declaraciones de flujo de control, incluidas declaraciones condicionales y bucles.

## Declaraciones condicionales

Las declaraciones condicionales se utilizan para tomar decisiones basadas en ciertas condiciones. Swift proporciona varias declaraciones condicionales, que incluyen:

### Sentencia if

La declaración if se usa para ejecutar un bloque de código si una determinada condición es verdadera. Esta es la sintaxis básica de una declaración if:

```swift
if condition {
    // Code to execute if the condition is true
}
```

Aquí hay un ejemplo del uso de una declaración if en Swift:

```swift
let age = 25

if age >= 18 {
    print("You are an adult")
}
```

### Declaración if-else

La declaración if-else se usa para ejecutar un bloque de código si una determinada condición es verdadera y otro bloque de código si la condición es falsa. Esta es la sintaxis básica de una instrucción if-else:

```swift
if condition {
    // Code to execute if the condition is true
} else {
    // Code to execute if the condition is false
}
```

Aquí hay un ejemplo del uso de una declaración if-else en Swift:

```swift
let age = 15

if age >= 18 {
    print("You are an adult")
} else {
    print("You are not an adult")
}
```

### Sentencia if-else-if

La declaración if-else-if se utiliza para ejecutar diferentes bloques de código en función de múltiples condiciones. Aquí está la sintaxis básica de una declaración if-else-if:

```swift
if condition1 {
    // Code to execute if condition1 is true
} else if condition2 {
    // Code to execute if condition2 is true
} else {
    // Code to execute if all conditions are false
}
```

Aquí hay un ejemplo del uso de una declaración if-else-if en Swift:

```swift
let grade = 85

if grade >= 90 {
    print("You got an A")
} else if grade >= 80 {
    print("You got a B")
} else if grade >= 70 {
    print("You got a C")
} else {
    print("You got a D or lower")
}
```

### Sentencia switch

La declaración de cambio se utiliza para ejecutar diferentes bloques de código en función de un valor determinado. Esta es la sintaxis básica de una sentencia switch:

```swift
switch value {
case value1:
    // Code to execute if value == value1
case value2:
    // Code to execute if value == value2
default:
    // Code to execute if value is not equal to any of the cases
}
```

Aquí hay un ejemplo del uso de una declaración de cambio en Swift:

```swift
let dayOfWeek = "Monday"

switch dayOfWeek {
case "Monday":
    print("It's Monday!")
case "Tuesday":
    print("It's Tuesday!")
case "Wednesday":
    print("It's Wednesday!")
case "Thursday":
    print("It's Thursday!")
case "Friday":
    print("It's Friday!")
default:
    print("It's the weekend!")
}
```

### Expresiones booleanas

Las expresiones booleanas son expresiones que se evalúan como un valor booleano (`true` o `false`). A menudo se usan en declaraciones condicionales para tomar decisiones basadas en ciertas condiciones. Swift proporciona varios operadores que se pueden usar para crear expresiones booleanas, que incluyen:

* Comparison operators: `==`, `!=`, `>`, `<`, `>=`, `<=`
* Logical operators: `&&` (logica AND), `||` (logica OR), `!` (logica NOT)

### Ejercicio: Calculadora de calificaciones

Cree un programa Swift que calcule la calificación de un estudiante en función de su puntaje porcentual. El programa debe solicitar al usuario el puntaje porcentual, luego usar declaraciones condicionales para determinar la calificación correspondiente según la siguiente escala:

* A: 90-100%
* B: 80-89%
* C: 70-79%
* D: 60-69%
* F: 0-59%

He aquí un ejemplo de cómo debería funcionar el programa:

```
Enter the percentage score: 85
Your grade is B
```

Para completar este ejercicio, deberá usar variables y constantes para almacenar la entrada del usuario y los valores calculados, declaraciones condicionales para determinar la calificación correspondiente según el puntaje porcentual e interpolación de cadenas para mostrar el resultado.

Aquí hay un código de inicio para ayudarlo a comenzar:

```
print("Enter the percentage score:")
// Use the readLine() function to read the user's input
// Store the percentage score in a variable or constant
// Use conditional statements to determine the corresponding grade
// Display the grade using string interpolation
```

¡Buena suerte y diviertete!
