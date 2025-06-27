
# Introducción a JavaScript y Uso de la Consola del Navegador

JavaScript es el lenguaje que permite a los desarrolladores agregar interactividad a las páginas web. A través de JavaScript, podemos responder a eventos, modificar el DOM (Document Object Model) y manejar datos dinámicos.

En esta clase, aprenderemos los fundamentos esenciales de JavaScript, empezando por cómo usar la consola para probar código en tiempo real. Los temas incluyen variables, condiciones, bucles, funciones, eventos, arrays y objetos.

## Uso de la Consola del Navegador

La **consola del navegador** es una herramienta de desarrollo que permite escribir, ejecutar y depurar código JavaScript en tiempo real. Puedes abrir la consola con los siguientes atajos:

- **Windows**: `Ctrl + Shift + I` o `F12`
- **Mac**: `Cmd + Option + I`

Una vez abierta la consola, puedes escribir código JavaScript y ver los resultados inmediatamente.

### Ejercicio Básico: Imprimir Mensajes en la Consola

Para empezar, escribe el siguiente código en la consola y presiona Enter:

```javascript
console.log("¡Hola, mundo!");
```

Esto mostrará el mensaje `"¡Hola, mundo!"` en la consola. `console.log()` es una función que nos permite imprimir información en la consola. A medida que avancemos, usaremos `console.log()` para ver los resultados de nuestro código.

## Variables en JavaScript

Las variables son contenedores que almacenan datos. Puedes crear variables con `let`, `var` o `const`.

### Ejemplo de Declaración de Variables

```javascript
let nombre = "Juan";  // let: la variable puede cambiar
const edad = 30;  // const: la variable es constante y no puede cambiar

console.log("Nombre:", nombre);
console.log("Edad:", edad);
```

#### Explicación de `let` y `const`

- **`let`**: Declara variables cuyo valor puede cambiar en el tiempo.
- **`const`**: Declara una constante, cuyo valor no puede modificarse después de ser definido.

**Prueba tú mismo:** Cambia el valor de `nombre` y observa cómo cambia el resultado en la consola.

## Tipos de Datos en JavaScript

JavaScript tiene varios tipos de datos básicos:

- `String` (texto)
- `Number` (números)
- `Boolean` (verdadero o falso)
- `Object` (objetos)
- `Array` (listas)

### Ejemplo de Diferentes Tipos de Datos

```javascript
let texto = "Hola, soy un texto";
let numero = 42;
let booleano = true;

console.log("Texto:", texto);
console.log("Número:", numero);
console.log("Booleano:", booleano);
```

**Prueba tú mismo:** Cambia los valores de `texto`, `numero` y `booleano` para experimentar con diferentes tipos de datos.

## Condiciones en JavaScript

Las condiciones permiten tomar decisiones dentro del código. La instrucción más común es `if`.

### Ejemplo de Uso de Condiciones

```javascript
let edad = prompt("Introduce tu edad:");
if (edad >= 18) {
    console.log("Eres mayor de edad");
} else {
    console.log("Eres menor de edad");
}
```

- **`if`**: Evalúa una condición, y si es verdadera, ejecuta el bloque de código asociado.
- **`else`**: Se ejecuta si la condición de `if` es falsa.

**Prueba tú mismo:** Introduce diferentes valores en el `prompt` para ver cómo cambia la salida en la consola.

## Bucles en JavaScript

Los bucles permiten ejecutar un bloque de código repetidas veces. Uno de los bucles más utilizados es el `for`.

### Ejemplo de Bucle `for`

```javascript
for (let i = 1; i <= 5; i++) {
    console.log(`Elemento ${i}`);
}
```

- **`for`**: Estructura de bucle que repite un bloque de código un número determinado de veces.

**Prueba tú mismo:** Cambia el valor final del bucle o el incremento (`i++`) para ver cómo afecta la salida.

## Funciones en JavaScript

Las funciones son bloques de código que pueden ser reutilizados en cualquier parte del programa.

### Ejemplo de Uso de Funciones

```javascript
function saludar(nombre) {
    return `Hola, ${nombre}!`;
}

let mensaje = saludar("Ana");
console.log(mensaje);
```

- **`function`**: Define una función.
- **`return`**: Devuelve un valor desde la función.

**Prueba tú mismo:** Llama a la función `saludar` con diferentes nombres.

### Funciones Anónimas

Las funciones anónimas son funciones sin nombre que pueden ser almacenadas en variables.

```javascript
let sumar = function(a, b) {
    return a + b;
};

console.log(sumar(3, 4));
```

**Prueba tú mismo:** Crea una función anónima para restar dos números.

## Eventos en JavaScript

Los eventos son interacciones que el usuario tiene con la página. Un evento común es hacer clic en un botón. En la consola, podemos simular estos eventos llamando directamente a las funciones.

### Ejemplo de Evento

```javascript
function mostrarAlerta() {
    alert("¡Has hecho clic en el botón!");
    console.log("Evento de clic ejecutado");
}
mostrarAlerta();
```

**Prueba tú mismo:** Modifica el mensaje de alerta y observa cómo cambia el comportamiento.

## Arrays en JavaScript

Un array es una lista de elementos. Cada elemento se almacena en una posición llamada índice.

### Ejemplo de Uso de Arrays

```javascript
let frutas = ["Manzana", "Banana", "Naranja"];
console.log("Primera fruta:", frutas[0]);
console.log("Todas las frutas:", frutas);
```

**Prueba tú mismo:** Añade más elementos al array y accede a ellos usando sus índices.

### Métodos de Array

Algunos métodos útiles para trabajar con arrays son `push`, `pop`, `shift` y `unshift`.

```javascript
frutas.push("Fresa");   // Añade un elemento al final
console.log("Después de push:", frutas);

frutas.pop();   // Elimina el último elemento
console.log("Después de pop:", frutas);
```

**Prueba tú mismo:** Experimenta con otros métodos como `shift` y `unshift`.

## Objetos en JavaScript

Un objeto es una colección de pares clave-valor. Cada clave tiene un valor asociado.

### Ejemplo de Uso de Objetos

```javascript
let persona = {
    nombre: "Juan",
    edad: 30,
    profesion: "Desarrollador"
};
console.log("Nombre:", persona.nombre);
console.log("Profesión:", persona.profesion);
```

**Prueba tú mismo:** Añade más propiedades al objeto y accede a ellas.

### Métodos en Objetos

Los objetos pueden tener métodos, que son funciones asociadas a ese objeto.

```javascript
let coche = {
    marca: "Toyota",
    modelo: "Corolla",
    arrancar: function() {
        console.log("El coche está arrancado");
    }
};

coche.arrancar();
```

**Prueba tú mismo:** Crea un método para detener el coche.


