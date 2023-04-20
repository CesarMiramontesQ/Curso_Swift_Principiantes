# Funciones y Cierres

En esta sección, profundizaremos en el concepto de funciones en Swift. Aprenderemos sobre diferentes tipos de funciones, incluidos los cierres, y exploraremos cómo usarlos en aplicaciones prácticas.

## Funciones

Una función es un bloque de código que realiza una tarea específica. Las funciones se utilizan para encapsular la lógica en componentes reutilizables, lo que hace que su código sea más modular y más fácil de mantener. Las funciones pueden tomar parámetros, que son entradas de la función, y devolver valores, que son salidas de la función.

### Definición de funciones

En Swift, las funciones se definen mediante la palabra clave `func`, seguida del nombre de la función, un conjunto de paréntesis que pueden contener uno o más parámetros y un tipo de devolución opcional. Aquí hay un ejemplo de una función simple en Swift que no toma parámetros y no devuelve ningún valor:

```swift
func sayHello() {
    print("Hello, world!")
}
```

### Llamando funciones

Para llamar a una función en Swift, simplemente use el nombre de la función seguido de un conjunto de paréntesis que pueden contener uno o más argumentos. Aquí hay un ejemplo de cómo llamar a la función `sayHello` desde arriba:

```swift
sayHello() // Output: "Hello, world!"
```

### Parámetros y valores devueltos

Las funciones también pueden tomar uno o más parámetros, que son entradas para la función. En Swift, los parámetros pueden tener valores predeterminados, ser variados (lo que significa que pueden tomar múltiples argumentos) e incluso pasarse por referencia usando la palabra clave `inout`. Aquí hay un ejemplo de una función en Swift que toma dos parámetros y devuelve su suma:

```swift
func addNumbers(_ a: Int, _ b: Int) -> Int {
    return a + b
}
```

La función anterior toma dos parámetros, `_ a: Int` y `_ b: Int`, y devuelve su suma como un valor Int.

### Parámetros Variádicos

Swift también admite parámetros variables, que le permiten pasar cualquier número de argumentos a una función. Los parámetros variádicos se indican con puntos suspensivos (`...`) después del tipo de parámetro. Aquí hay un ejemplo de una función que toma un parámetro variádico y devuelve su suma:

```swift
func addNumbers(_ numbers: Int...) -> Int {
    return numbers.reduce(0, +)
}
```

La función anterior toma cualquier cantidad de argumentos `Int` y devuelve su suma como un valor `Int`.

## Cierres

Los cierres son similares a las funciones, pero pueden pasarse como variables y usarse de formas más flexibles. Los cierres se utilizan a menudo para el manejo de eventos y para implementar patrones de programación funcional. En Swift, los cierres se definen usando una sintaxis similar a las funciones, pero con llaves en lugar de paréntesis.

### Definición de cierres

Aquí hay un ejemplo de un cierre en Swift que toma dos números enteros como parámetros y devuelve su suma:

```swift
let addNumbers = { (a: Int, b: Int) -> Int in
    return a + b
}
```

### Llamando cierres

Para llamar a un cierre en Swift, usa el nombre de la variable de cierre seguido de un conjunto de paréntesis que pueden contener uno o más argumentos. Aquí hay un ejemplo de cómo llamar al cierre `addNumbers` desde arriba:

```swift
let result = addNumbers(1, 2) // result = 3
```

### Capturando valores

Los cierres también pueden capturar valores de su contexto circundante. Esto significa que pueden acceder y modificar variables que se definen fuera del cierre. Aquí hay un ejemplo de un cierre que captura un valor:

```swift
var counter = 0
let incrementCounter = {
    counter += 1
}
incrementCounter() // counter = 1
incrementCounter() // counter = 2
incrementCounter() // counter = 3
```

## Ejercicio: Funciones y Cierres

1. Defina una función llamada `calculateAverage` que tome una matriz de enteros como parámetro y devuelva el promedio de esos números como un `Doble`.
2. Defina un cierre llamado `sortAscending` que tome dos enteros como parámetros y devuelva `true` si el primer entero es menor que el segundo entero, y `false` en caso contrario.
3. Defina un cierre llamado `sortDescending` que tome dos enteros como parámetros y devuelva `true` si el primer entero es mayor que el segundo entero, y `false` en caso contrario.
4. Cree un arreglo de enteros y use la función de `calculateAverage` para calcular el promedio del arreglo.
5. Cree un nuev arreglos de enteros y use el método `sorted(by:)` para ordenar el arreglo en orden ascendente usando el cierre `sortAscending`.
6. Cree otra arreglo de enteros y utilice el método `sorted(by:)` para ordenar la matriz en orden descendente utilizando el cierre `sortDescending`.

Sugerencia: el método `sorted(by:)` toma un cierre que define los criterios de clasificación para el arreglo. El cierre debe tomar dos argumentos del mismo tipo que el del arreglo y devolver un valor `Bool` que indica si el primer argumento debe ordenarse antes que el segundo argumento.

Por ejemplo, para ordenar una matriz de números enteros en orden ascendente, podría usar el siguiente cierre:

```swift
let sortAscending = { (a: Int, b: Int) -> Bool in
    return a < b
}
```
