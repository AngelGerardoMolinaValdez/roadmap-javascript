# Variables (var, let, const) en JavaScript 👩‍💻

Las variables son espacios de memoria que se referencian de un identificador. Este identificador es una palabra que se rige de una seria de reglas por ejemplo:
- El primer carácter debe ser una letra
- No se pueden agregar espacios entre letras
- Solo se aceptan los caracteres [a-z_A-Z_\__0-9]

Ejemplos validos:
- nombre_completo
- x
- OTRO_DATO

Ejemplos incorrectos:
- 1_usuario
- edad-usuario
- dirección usuario

Gracias a estos identificadores podemos acceder las veces que sean necesarias
a dicho espacio en memoria y modificar su valor.

## Declaración
Se pueden declarar variables usando las palabras clave `var`, `let`, o `const`.
- `var`: Es la forma mas antigua que Javascript tiene para definir variables, esta declaración puede ocasionar problemas por como se crean las variables por el "scope"
- `let`: Permite declarar variables con alcance de bloque, lo que es más predecible que `var`.
- `const`: Se utiliza para declarar variables cuyos valores no deben ser reasignados después de su inicialización.

```javascript
var oldVariable = 'old'; // Not recommended
let newVariable = 'new'; // Recommended
const constantVariable = 'constant'; // Recommended for constants
```

## Alcance (Scope)
El alcance de una variable se refiere a la parte del código donde está disponible para su uso.
- `var` tiene un alcance funcional.
- `let` y `const` tienen un alcance de bloque.

```javascript
function example() {
  if (true) {
    var varScope = 'function scope';
    let blockScope = 'block scope';
  }
  console.log(varScope); // Logs 'function scope'
  console.log(blockScope); // Error: blockScope is not defined
}
```

## Hoisting
"Hoisting" es un mecanismo en JavaScript donde las variables y las declaraciones de funciones se mueven al principio de su código o al principio de su función antes de la ejecución del código.
- Las variables declaradas con `var` son "hoisted" con un valor de `undefined`.
- Las variables declaradas con `let` y `const` también son "hoisted" pero no son inicializadas.

```javascript
console.log(hoistedVar); // Logs 'undefined'
var hoistedVar = 'I am hoisted';
```

## Conclusiones
La comprensión del alcance y el hoisting es importante para evitar errores y escribir código predecible y mantenible. Es aconsejable utilizar `let` y `const` en lugar de `var` en código moderno para una mejor claridad y seguridad en el manejo de datos.

## Referencias

[developer.mozilla.org - Variables](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables)

[developer.mozilla.org - Var](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var)

[developer.mozilla.org - Let](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)

[developer.mozilla.org- Const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const?ref=thomasclowes.com)


## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/02-variables-y-tipos-de-datos/variables-var-let-const.md)

[🏡 Volver al inicio](../../readme.md)