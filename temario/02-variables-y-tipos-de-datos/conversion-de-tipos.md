# Conversión de Tipos en JavaScript 👩‍💻

Al proceso de convertir un tipo de dato con otro se le llama coercion, esta conversion debe ser entre datos compatibles ejemplo String y Number, Number y Boolean, etc.

JavaScript permite la conversión entre diferentes tipos de datos. Esto puede ocurrir de manera explícita (coerción explícita) o implícita (coerción implícita).

## Coercion Explicita
La coerción explícita ocurre cuando el programador indica de manera clara y directa que desea convertir un valor de un tipo de datos a otro. Esto se logra a través de funciones y métodos específicos proporcionados por el lenguaje.

**Ejemplo**:
```javascript
let str = String(123); // convierte número a string
let num = Number('123'); // convierte string a número
```

## Coercion Implícita
La coerción implícita ocurre cuando JavaScript convierte automáticamente un tipo de dato a otro sin que el programador lo indique explícitamente. Esto puede ocurrir, por ejemplo, cuando se están realizando operaciones entre diferentes tipos de datos. El lenguaje intentará hacer una conversión automática para que la operación se pueda llevar a cabo.

**Ejemplo**:
```javascript
let result = '123' + 456; // result será '123456' como string
```

## Referencias
[developer.mozilla.org - coercion](https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion)

[freecodecamp.org - coercion](https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/02-variables-y-tipos-de-datos/conversion-de-tipos.md)

[🏡 Volver al inicio](../../readme.md)