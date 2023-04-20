# Parámetros y valores devueltos

En esta sección, aprenderemos sobre los parámetros y los valores devueltos en las funciones de Swift. Exploraremos cómo pasar parámetros a funciones, cómo devolver valores de funciones y cómo usar valores de parámetros predeterminados, parámetros variádicos y parámetros de `inout`.

## Parámetros de función

Un parámetro es un valor que se pasa a una función para ser utilizado dentro de la función. En Swift, puede definir uno o más parámetros en la lista de parámetros de la función. He aquí un ejemplo de una función que toma dos parámetros:

```swift
func greet(name: String, message: String) {
    print("\(name), \(message)")
}
```

La función anterior toma dos parámetros, `name` y `message`, ambos de tipo `String`. Para llamar a esta función, pasaría dos valores de cadena:

```swift
greet(name: "John", message: "how are you?")
```

Esto daría como resultado:

```
John, how are you?
```

## Valores de regreso en una función

Una función también puede devolver un valor usando la palabra clave `return`. Aquí hay un ejemplo de una función que devuelve un valor `Int`:

```swift
func addNumbers(a: Int, b: Int) -> Int {
    return a + b
}
```

La función anterior toma dos parámetros, `a` y `b`, ambos de tipo `Int`, y devuelve su suma como un valor `Int`.

Para llamar a esta función y recuperar el valor de retorno, haría lo siguiente:

```swift
let result = addNumbers(a: 2, b: 3)
print(result)
```

Esto daría como resultado:

```swift
5
```

## Valores de parámetros predeterminados

En Swift, también puede especificar valores de parámetros predeterminados para una función. Esto le permite llamar a la función sin pasar un valor para ese parámetro, y usará el valor predeterminado en su lugar. Aquí hay un ejemplo de una función que toma un valor de parámetro predeterminado:

```swift
func greet(name: String, message: String = "hello") {
    print("\(name), \(message)")
}
```

La función anterior toma dos parámetros, `name` y `mensage`, y el mensaje tiene un valor predeterminado de "hello". Esto significa que si llama a la función sin pasar un valor para el mensaje, usará el valor predeterminado:

```swift
greet(name: "John") // Output: John, hello
```
## Parámetros Variádicos

Swift también admite parámetros variables, que le permiten pasar cualquier cantidad de valores a una función. Los parámetros variádicos se indican con puntos suspensivos (`...`) después del tipo de parámetro. Aquí hay un ejemplo de una función que toma un parámetro variádico:

```swift
func sum(numbers: Int...) -> Int {
    var result = 0
    for number in numbers {
        result += number
    }
    return result
}
```

La función anterior toma `numbers` de parámetros variables, que es una lista de valores `Int`. Luego, la función suma todos los valores de la lista y devuelve el total.

Para llamar a esta función, puede pasar cualquier número de valores `Int`:

```swift
let total = sum(numbers: 1, 2, 3, 4)
print(total) // Output: 10
```

## Parametros Inout

En Swift, los parámetros se pasan por valor de forma predeterminada, lo que significa que se pasa una copia del valor del parámetro a la función. Sin embargo, también puede pasar parámetros por referencia utilizando la palabra clave `inout`. Esto permite que la función modifique el valor del parámetro directamente.

Aquí hay un ejemplo de una función que toma un parámetro de `inout`:

```swift
func swapValues(a: inout Int,
```

## Ejercicio: Parámetros y Valores de Retorno

1. Defina una función llamada `calculeRectangleArea` que tome dos parámetros, `width` y `height`, ambos de tipo `Doble`, y devuelva el área de un rectángulo como `Doble`.
2. Defina una función denominada `calcularCirculoCircunferencia` que tome un parámetro, `radius`, de tipo `Doble`, y devuelva la circunferencia de un círculo como `Doble`. Use el valor de Pi (3.14159265) para el cálculo.
3. Defina una función llamada `calculeTriangleArea` que tome dos parámetros, `base` y `height`, ambos de tipo `Double`, y devuelva el área de un triángulo como `Double`.
4. Defina una función llamada `greet` que tome dos parámetros, `name` y `age`, ambos de tipo `String`, y devuelva un mensaje de saludo como un `String`. El mensaje de saludo debe tener el formato "Hello, [name], you are [age] years old.".

Sugerencia: para calcular el área de un rectángulo, puede usar la fórmula `área = ancho * alto`. Para calcular la circunferencia de un círculo, puedes usar la fórmula `circunferencia = 2 * Pi * radio`. Para calcular el área de un triángulo, puedes usar la fórmula `área = 0,5 * base * altura`.

