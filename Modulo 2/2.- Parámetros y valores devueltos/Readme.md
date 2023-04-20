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

