# Bucles y arreglos

Los bucles se utilizan para repetir un bloque de código varias veces, mientras que las matrices se utilizan para almacenar colecciones de datos.

## Estructuras de bucle en Swift

Swift proporciona varias estructuras de bucle, que incluyen:

### Bucle for-in

El bucle for-in se usa para iterar sobre una colección de datos, como una matriz o un rango de números. Esta es la sintaxis básica de un bucle for-in:

```swift
for item in collection {
    // Code to execute for each item in the collection
}
```

Aquí hay un ejemplo del uso de un bucle for-in en Swift para imprimir los elementos de una matriz:

```swift
let numbers = [1, 2, 3, 4, 5]

for number in numbers {
    print(number)
}
```

### Bucle While

El bucle while se utiliza para repetir un bloque de código mientras se cumple una determinada condición. Esta es la sintaxis básica de un ciclo while:

```swift
while condition {
    // Code to execute while the condition is true
}
```

Aquí hay un ejemplo del uso de un bucle while en Swift para imprimir los números del 1 al 5:

```swift
var i = 1

while i <= 5 {
    print(i)
    i += 1
}
```

### Bucle repeat-while

El bucle repeat-while es similar al bucle while, pero siempre ejecuta el código al menos una vez, incluso si la condición es falsa. Aquí está la sintaxis básica de un ciclo de repetición mientras:

```swift
repeat {
    // Code to execute at least once
} while condition
```

Aquí hay un ejemplo del uso de un bucle de repetición en Swift para imprimir los números del 1 al 5:

```swift
var i = 1

repeat {
    print(i)
    i += 1
} while i <= 5
```

### Arreglos

Una matriz es una colección de datos que puede contener múltiples valores del mismo tipo. Así es como puede declarar una matriz en Swift:

```swift
let array = [value1, value2, value3, ...]
```

Aquí hay un ejemplo de cómo declarar una matriz de enteros en Swift:

```swift
let numbers = [1, 2, 3, 4, 5]
```

Puede acceder a los elementos de una matriz usando su índice, que comienza en 0. Así es como puede acceder al primer elemento de una matriz en Swift:

```swift
let firstNumber = numbers[0]
```

También puede modificar los elementos de una matriz utilizando su índice. Así es como puede cambiar el valor del primer elemento de una matriz en Swift:

```swift
numbers[0] = 10
```

Finalmente, puede iterar sobre los elementos de una matriz utilizando un bucle for-in. Así es como puede imprimir los elementos de una matriz usando un bucle for-in en Swift:

```swift
for number in numbers {
    print(number)
}
```

### Conclusion

Los bucles y las matrices son conceptos importantes en la programación y se utilizan en una amplia variedad de aplicaciones. Al comprender cómo usar bucles para iterar sobre colecciones de datos y cómo declarar y manipular matrices, puede convertirse en un programador más eficaz y eficiente.

### Ejercicio: Suma de Números Pares

Cree un programa Swift que calcule la suma de todos los números pares en una matriz de enteros. El programa debe solicitar al usuario el tamaño de la matriz y los valores de la matriz, luego usar un ciclo para iterar sobre los elementos de la matriz y sumar los números pares.

He aquí un ejemplo de cómo debería funcionar el programa:

```swift
Enter the size of the array: 6
Enter the values of the array: 1 2 3 4 5 6
The sum of even numbers is 12
```

Para completar este ejercicio, deberá usar variables y constantes para almacenar la entrada del usuario y los valores calculados, un ciclo para iterar sobre los elementos de la matriz y declaraciones condicionales para verificar si cada elemento es par.

Aquí hay un código de inicio para ayudarlo a comenzar:

```swift
print("Enter the size of the array:")
// Use the readLine() function to read the user's input
// Store the size of the array in a variable or constant
// Create an empty array of integers
// Use a loop to prompt the user for the values of the array
// Store the values in the array
// Use a loop to iterate over the elements of the array
// Use conditional statements to check whether each element is even
// If the element is even, add it to a variable that stores the sum of even numbers
// Display the sum of even numbers using string interpolation
```

¡Buena suerte y diviertete!
