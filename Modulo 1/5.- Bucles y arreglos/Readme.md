# Bucles y arreglos

En este módulo, los estudiantes aprenderán sobre los fundamentos de los bucles y los arreglos en Swift. A continuación, se explican los temas principales que se tratarán en este módulo:

## Estructuras de bucle en Swift

En este tema, los estudiantes aprenderán sobre las diferentes estructuras de bucle en Swift, como for-in, while y repeat-while. Se les mostrará cómo utilizar estas estructuras de bucle para iterar sobre colecciones de datos y realizar operaciones repetitivas.

```swift
// for-in loop
for numero in 1...5 {
    print(numero)
}

// while loop
var i = 1
while i <= 5 {
    print(i)
    i += 1
}

// repeat-while loop
var j = 1
repeat {
    print(j)
    j += 1
} while j <= 5
```

## Declaración y manipulación de arreglos

En este tema, los estudiantes aprenderán a declarar y manipular arreglos en Swift. Se les mostrará cómo crear y declarar un arreglo, y cómo agregar, eliminar y acceder a elementos dentro de un arreglo. También aprenderán sobre las funciones de alto nivel disponibles en Swift para trabajar con arreglos, como filter y map.

```swift
// Crear un arreglo
var numeros = [1, 2, 3, 4, 5]

// Agregar un elemento al arreglo
numeros.append(6)

// Acceder a un elemento del arreglo
let tercerNumero = numeros[2]

// Eliminar un elemento del arreglo
numeros.remove(at: 3)

// Iterar sobre un arreglo utilizando for-in loop
for numero in numeros {
    print(numero)
}

// Utilizar la función filter en un arreglo
let numerosPares = numeros.filter { $0 % 2 == 0 }
print(numerosPares)

// Utilizar la función map en un arreglo
let numerosCuadrados = numeros.map { $0 * $0 }
print(numerosCuadrados)
```

## Bucles anidados

En este tema, los estudiantes aprenderán sobre los bucles anidados en Swift. Se les mostrará cómo utilizar bucles anidados para iterar sobre colecciones de datos de múltiples dimensiones, como matrices y matrices anidadas.

```swift
// Declarar una matriz bidimensional
let matriz = [[1, 2], [3, 4], [5, 6]]

// Iterar sobre la matriz utilizando bucles anidados
for fila in matriz {
    for numero in fila {
        print(numero)
    }
}
```

En general, este módulo proporcionará a los estudiantes una comprensión sólida de los bucles y los arreglos en Swift. Al final de este módulo, los estudiantes tendrán las habilidades necesarias para utilizar las estructuras de bucle de Swift, como for-in, while y repeat-while, para iterar sobre colecciones de datos, y también sabrán cómo declarar y manipular arreglos en Swift.


## Ejercicio: Suma de Números Pares

Cree un programa Swift que calcule la suma de todos los números pares en una matriz de enteros. El programa debe solicitar al usuario el tamaño de la matriz y los valores de la matriz, luego usar un ciclo para iterar sobre los elementos de la matriz y sumar los números pares.

Aquí un ejemplo de cómo debería funcionar el programa:

```swift
Introduzca el tamaño de la matriz: 6
Introduzca los valores de la matriz: 1 2 3 4 5 6
la suma de los numeros pares es 12
```

Para completar este ejercicio, deberá usar variables y constantes para almacenar la entrada del usuario y los valores calculados, un ciclo para iterar sobre los elementos de la matriz y declaraciones condicionales para verificar si cada elemento es par.

Aquí hay un código de inicio para ayudarlo a comenzar:

```swift
print("Ingrese el tamaño de la matriz:")
// Usa la función readLine() para leer la entrada del usuario
// Almacenar el tamaño de la matriz en una variable o constante
// Crea una matriz vacía de enteros
// Usar un bucle para solicitar al usuario los valores de la matriz
// Almacenar los valores en la matriz
// Usa un bucle para iterar sobre los elementos de la matriz
// Usa sentencias condicionales para verificar si cada elemento es par
// Si el elemento es par, añádelo a una variable que almacene la suma de números pares
// Muestra la suma de los números pares usando la interpolación de cadenas
```
