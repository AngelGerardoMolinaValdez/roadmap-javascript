# Tipos de Datos en JavaScript 👩‍💻

## Definición
Los datos son piezas de información que pueden ser manipuladas y gestionadas en un programa. Los datos pueden representar varias cosas, por ejemplo Números como 5, 10.5, textos como "Hola Mundo", imágenes, sonidos, etc.

Los tipos de datos son categorías para los datos que permiten a los programas saber cómo deben manejar diferentes piezas de información.

## Tipos de datos primitivos
Los datos primitivos son los tipos de datos más básicos que proporciona un lenguaje de programación. En JavaScript, estos incluyen `Number`, `String`, `Boolean`, `null`, `undefined`, y `Symbol`. Son inmutables y se comparan por su valor.

## Tipos de datos compuestos
Los datos compuestos o estructurados, son tipos de datos que agrupan otros datos, ya sean primitivos o incluso otros datos compuestos. En JavaScript, los objetos y arrays son ejemplos de datos compuestos. Los datos compuestos son mutables y se comparan por su referencia en memoria, no por su valor.

## Number
Este tipo de dato es usado para representar números, ya sean enteros o flotantes (decimales).

**Ejemplo**:
```javascript
let age = 25; // un número entero
let pi = 3.14159; // un número flotante
```

## String
El tipo de dato string es usado para representar texto. Puede ser creado usando comillas simples, dobles o back-ticks.

**Ejemplo**:
```javascript
let name = 'John Doe'; // usando comillas simples
let greeting = "Hello"; // usando comillas dobles
let phrase = `Hello, ${name}`; // usando back-ticks para interpolación de strings
```

## Boolean
El tipo de dato booleano representa verdadero o falso, y es útil para controlar el flujo de un programa con estructuras condicionales.

**Ejemplo**:
```javascript
let isAdult = true;
let isStudent = false;
```

## null
El valor `null` representa una ausencia intencional de valor. Es un valor que representa "nada" o "vacío".

**Ejemplo**:
```javascript
let emptyValue = null;
```

## undefined
El valor `undefined` es asignado automáticamente a las variables que han sido declaradas, pero que aún no han sido inicializadas con un valor.

**Ejemplo**:
```javascript
let notDefined;
console.log(notDefined); // output: undefined
```

## Object
Los objetos son colecciones de pares clave-valor y son usados para representar estructuras de datos complejas.

**Ejemplo**:
```javascript
let person = {
    name: 'John Doe',
    age: 25,
    isAdult: true
};
```

## Symbol
Un tipo de dato que proporciona una manera de crear valores únicos.

**Ejemplo**:
```javascript
const uniqueSymbol = Symbol('description');
```

## Conversión entre Tipos (Coerción)
Al proceso de convertir un tipo de dato con otro se le llama coercion, esta conversion debe ser entre datos compatibles ejemplo String y Number, Number y Boolean, etc.

JavaScript permite la conversión entre diferentes tipos de datos. Esto puede ocurrir de manera explícita (coerción explícita) o implícita (coerción implícita).

### Coercion Explicita
La coerción explícita ocurre cuando el programador indica de manera clara y directa que desea convertir un valor de un tipo de datos a otro. Esto se logra a través de funciones y métodos específicos proporcionados por el lenguaje.

**Ejemplo**:
```javascript
let str = String(123); // convierte número a string
let num = Number('123'); // convierte string a número
```

### Coercion Implícita
La coerción implícita ocurre cuando JavaScript convierte automáticamente un tipo de dato a otro sin que el programador lo indique explícitamente. Esto puede ocurrir, por ejemplo, cuando se están realizando operaciones entre diferentes tipos de datos. El lenguaje intentará hacer una conversión automática para que la operación se pueda llevar a cabo.

**Ejemplo**:
```javascript
let result = '123' + 456; // result será '123456' como string
```

## Referencias

[developer.mozilla.org - tipos de datos](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)

[developer.mozilla.org - coercion](https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion)

[freecodecamp.org - coercion](https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/02-variables-y-tipos-de-datos/tipos-de-datos.md)

[🏡 Volver al inicio](../../readme.md)