# Módulo 2: Funciones y Opcionales

En este módulo, los estudiantes aprenderán cómo definir y usar funciones en Swift, que son bloques de código reutilizables que realizan una tarea específica. También aprenderán sobre los cierres, que son similares a las funciones pero se pueden pasar como variables. Además, los estudiantes aprenderán cómo usar opciones en Swift para manejar situaciones en las que un valor puede estar presente o no, y cómo usar el manejo de errores para manejar correctamente errores inesperados.

## Funciones y Cierres

Las funciones son un concepto fundamental en la programación y se utilizan para encapsular un bloque de código que realiza una tarea específica. En Swift, las funciones pueden tomar parámetros, devolver valores e incluso anidarse dentro de otras funciones.

### Definición de funciones

Esta es la sintaxis básica para definir una función en Swift:

```swift
func functionName(parameter1: Type, parameter2: Type, ...) -> ReturnType {
    // Code to execute when the function is called
    return returnValue
}
```

Aquí hay un ejemplo de una función en Swift que toma dos números enteros como parámetros y devuelve su suma:

```swift
func addNumbers(_ a: Int, _ b: Int) -> Int {
    return a + b
}
```

### Cierres

Los cierres son similares a las funciones, pero pueden pasarse como variables y usarse de formas más flexibles. En Swift, los cierres se definen usando una sintaxis similar a las funciones, pero con llaves en lugar de paréntesis.

Aquí hay un ejemplo de un cierre en Swift que toma dos números enteros como parámetros y devuelve su suma:

```swift
let addNumbers = { (a: Int, b: Int) -> Int in
    return a + b
}
```

## Parámetros y valores devueltos

En esta sección, los estudiantes aprenderán cómo pasar parámetros a funciones y cómo devolver valores de funciones. También aprenderán sobre los valores de los parámetros predeterminados, los parámetros variádicos y los parámetros de entrada y salida.

### Parameters

Los parámetros se utilizan para pasar datos a las funciones. En Swift, los parámetros pueden tener valores predeterminados, ser variados (lo que significa que pueden tomar múltiples argumentos) e incluso pasarse por referencia usando la palabra clave `inout`.

Aquí hay un ejemplo de una función en Swift que toma dos números enteros como parámetros y devuelve su suma:

```swift
func addNumbers(_ a: Int, _ b: Int) -> Int {
    return a + b
}
```

### Valores devueltos

Las funciones también pueden devolver valores, que se utilizan para devolver datos al código de llamada. En Swift, las funciones pueden devolver cualquier tipo, incluidas otras funciones o cierres.

Aquí hay un ejemplo de una función en Swift que devuelve un cierre:

```swift
func getAddFunction() -> ((Int, Int) -> Int) {
    return { (a: Int, b: Int) -> Int in
        return a + b
    }
}
```

## Opcionales y Desembalaje

En esta sección, los estudiantes aprenderán sobre las opciones en Swift, que se utilizan para manejar situaciones en las que un valor puede o no estar presente. También aprenderán cómo desenvolver opcionales para acceder a sus valores subyacentes y cómo usar el encadenamiento opcional para acceder de manera segura a los opcionales anidados.

### Opcionales

En Swift, un opcional es un tipo que puede tener un valor o ser nulo. Esto es útil para manejar situaciones en las que un valor puede o no estar presente, como cuando se analizan datos de una fuente externa.

Aquí hay un ejemplo de un opcional en Swift:

```swift
let optionalValue: Int? = 5
```

### Desempaquetar Opcionales

Para acceder al valor subyacente de un opcional, se debe desenvolver. En Swift, esto se suele hacer mediante un enlace opcional, que

## Manejo de errores

En esta sección, los estudiantes aprenderán sobre el manejo de errores en Swift, que se usa para manejar errores inesperados que pueden ocurrir durante la ejecución del programa. Aprenderán cómo definir y lanzar errores usando la palabra clave `throws`, y cómo manejar los errores usando los bloques `try`, `catch` y `finally`

### Throwing Errors

En Swift, los errores se representan mediante el protocolo `Error`, que define la estructura básica de un `error`. Para definir un error personalizado, puede crear un nuevo tipo que se ajuste al protocolo de error.

Aquí hay un ejemplo de cómo definir un error personalizado en Swift:

```swift
enum NetworkError: Error {
    case badRequest
    case unauthorized
    case notFound
    case serverError
}
```

Para arrojar un error en Swift, puede usar la palabra clave throw seguida del error que desea arrojar. Aquí hay un ejemplo de arrojar un error en Swift:

```swift
func fetchData(url: URL) throws -> Data {
    let session = URLSession.shared
    let request = URLRequest(url: url)
    var data: Data?
    var error: Error?
    let semaphore = DispatchSemaphore(value: 0)
    let task = session.dataTask(with: request) { (responseData, _, responseError) in
        data = responseData
        error = responseError
        semaphore.signal()
    }
    task.resume()
    semaphore.wait()
    if let error = error {
        throw error
    } else if let data = data {
        return data
    } else {
        throw NetworkError.serverError
    }
}
```

### Manejo de errores

Para manejar errores en Swift, puede usar un bloque `do`-`catch, el bloque `do` contiene el código que puede arrojar un error, y el bloque `catch` contiene el código para manejar el error si ocurre.

Aquí hay un ejemplo de manejo de un error en Swift:

```swift
let url = URL(string: "https://example.com/data")!
do {
    let data = try fetchData(url: url)
    print(String(data: data, encoding: .utf8)!)
} catch NetworkError.badRequest {
    print("Bad request")
} catch NetworkError.unauthorized {
    print("Unauthorized")
} catch NetworkError.notFound {
    print("Not found")
} catch NetworkError.serverError {
    print("Server error")
} catch {
    print("An error occurred: \(error)")
}
```

Además de los bloques `do`-`catch`, Swift también admite un bloque `finally`, que se ejecuta independientemente de si se arroja un error o no. Esto puede ser útil para realizar tareas de limpieza, como cerrar archivos o liberar recursos.

Aquí hay un ejemplo del uso de un bloque `finally` en Swift:

```swift
let file = try File(path: "data.txt")
do {
    let data = try file.readData()
    print(String(data: data, encoding: .utf8)!)
} catch {
    print("An error occurred: \(error)")
} finally {
    file.close()
}
```

## Conclusion

Las funciones y los opcionales son conceptos fundamentales en Swift y se usan ampliamente en la programación de Swift. Al comprender cómo definir y usar funciones, cómo trabajar con opciones y cómo manejar errores en Swift, puede convertirse en un programador de Swift más eficaz y eficiente.
