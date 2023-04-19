# Flujo de control y sentencias condicionales

En este módulo, los estudiantes aprenderán sobre el flujo de control y las sentencias condicionales en Swift. A continuación, se explican los temas principales que se tratarán en este módulo:

## Sentencia if

En este tema, los estudiantes aprenderán sobre la sentencia if en Swift, que se utiliza para tomar decisiones basadas en una condición. Se les mostrará cómo utilizar la sentencia if para evaluar una expresión booleana y ejecutar un bloque de código si la expresión es verdadera.

```swift
var edad = 18

if edad >= 18 {
    print("Eres mayor de edad")
} else {
    print("Eres menor de edad")
}
```

## Sentencia else-if

En este tema, los estudiantes aprenderán acerca de la sentencia else-if en Swift, que se utiliza para evaluar múltiples condiciones en una estructura if. Se les mostrará cómo utilizar la sentencia else-if para evaluar varias expresiones booleanas y ejecutar un bloque de código si se cumple una de las condiciones.

```swift
var puntaje = 85

if puntaje >= 90 {
    print("Excelente trabajo!")
} else if puntaje >= 80 {
    print("Muy bien!")
} else if puntaje >= 70 {
    print("Bien hecho")
} else {
    print("Debes mejorar")
}
```

## Sentencia switch-case

En este tema, los estudiantes aprenderán acerca de la sentencia switch-case en Swift, que se utiliza para evaluar múltiples condiciones y ejecutar diferentes bloques de código en función de las condiciones evaluadas. Se les mostrará cómo utilizar la sentencia switch-case para evaluar diferentes expresiones y ejecutar diferentes bloques de código en función de los resultados.

```swift
var diaSemana = 3

switch diaSemana {
case 1:
    print("Hoy es Lunes")
case 2:
    print("Hoy es Martes")
case 3:
    print("Hoy es Miércoles")
case 4:
    print("Hoy es Jueves")
case 5:
    print("Hoy es Viernes")
case 6:
    print("Hoy es Sábado")
case 7:
    print("Hoy es Domingo")
default:
    print("Día no válido")
}
```

## Expresiones booleanas

En este tema, los estudiantes aprenderán sobre las expresiones booleanas en Swift, que se utilizan en las sentencias condicionales para evaluar si una condición es verdadera o falsa. Se les mostrará cómo utilizar diferentes operadores lógicos para crear expresiones booleanas más complejas.

```swift
var nota = 8

if nota >= 7 && nota <= 10 {
    print("Aprobado")
} else if nota >= 4 && nota < 7 {
    print("Regular")
} else if nota >= 0 && nota < 4 {
    print("Reprobado")
} else {
    print("Nota inválida")
}
```

En general, este módulo proporcionará a los estudiantes una comprensión sólida del flujo de control y las sentencias condicionales en Swift. Al final de este módulo, los estudiantes tendrán las habilidades necesarias para utilizar las sentencias condicionales de Swift, como if, else-if y switch-case, para tomar decisiones basadas en ciertas condiciones, y también sabrán cómo utilizar expresiones booleanas en las sentencias condicionales.

## Ejercicio: Calculadora de calificaciones

Cree un programa Swift que calcule la calificación de un estudiante en función de su puntaje porcentual. El programa debe solicitar al usuario el puntaje porcentual, luego usar declaraciones condicionales para determinar la calificación correspondiente según la siguiente escala:

* A: 90-100%
* B: 80-89%
* C: 70-79%
* D: 60-69%
* F: 0-59%

He aquí un ejemplo de cómo debería funcionar el programa:

```swift
Ingresa la calificacion: 85
Tu calificacion es B
```

Para completar este ejercicio, deberá usar variables y constantes para almacenar la entrada del usuario y los valores calculados, declaraciones condicionales para determinar la calificación correspondiente según el puntaje porcentual e interpolación de cadenas para mostrar el resultado.

Aquí hay un código de inicio para ayudarlo a comenzar:

```swift
print("Ingresa la calificacion:")
// Use the readLine() function to read the user's input
// Store the percentage score in a variable or constant
// Use conditional statements to determine the corresponding grade
// Display the grade using string interpolation
```
