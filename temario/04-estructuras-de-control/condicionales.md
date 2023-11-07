# Estructuras de control condicionales en JavaScript 👩‍💻

Los condicionales son estructuras de control que permiten ejecutar diferentes acciones según se cumplan o no determinadas condiciones. Son fundamentales para la toma de decisiones dentro de tus programas. Dirigen el flujo de ejecución en un programa basándose en evaluaciones. Estas evaluaciones resultan en valores lógicos o booleanos (`true` o `false`)

## If/Else

Permite ejecutar un bloque de código si, y solo si, una condición específica es verdadera.

```javascript
if (condición) {
  // Código a ejecutar si la condición es verdadera
}
```

Para acciones alternativas, se usa `else`:

```javascript
if (condición) {
  // Código si la condición es verdadera
} else {
  // Código si la condición es falsa
}
```

Y para múltiples condiciones, se utiliza `else if`:

```javascript
if (condición1) {
  // Código si condición1 es verdadera
} else if (condición2) {
  // Código si condición2 es verdadera
} else {
  // Código si ninguna condición anterior se cumple
}
```

## Switch

La declaración switch es una alternativa a if cuando tienes múltiples condiciones que dependen del mismo valor. Es particularmente útil y más legible cuando se comparan la misma variable o expresión con diferentes valores.

```javascript
switch (expresión) {
  case valor1:
    // Código si expresión === valor1
    break;
  case valor2:
    // Código si expresión === valor2
    break;
  default:
    // Código si no hay coincidencia con ningún caso
}
```

Cada caso se compara con la expresión utilizando una comparación estricta (===), y si se encuentra una coincidencia, se ejecuta el bloque de código asociado. El break es crucial para evitar que la ejecución se "deslice" hacia el siguiente caso (fall-through). El caso default es opcional y se ejecuta si ningún otro caso coincide.

## Condicionales compuestas y anidadas
Las condiciones compuestas y anidadas son técnicas avanzadas que permiten manejar escenarios lógicos complejos de manera eficiente y legible

### Condiciones Compuestas

Las condiciones compuestas utilizan operadores lógicos para combinar varias condiciones en una única declaración. Los operadores lógicos más comunes son:

- `&&` (AND): Evalúa si todas las condiciones son verdaderas.
- `||` (OR): Evalúa si al menos una de las condiciones es verdadera.
- `!` (NOT): Niega la condición, invirtiendo su resultado de verdadero a falso o viceversa.

Un ejemplo de una condición compuesta es:

```javascript
if (condicion1 && condicion2) {
  // El código se ejecuta si tanto condicion1 como condicion2 son verdaderas
}
```

Estas estructuras son cruciales cuando se necesitan realizar una acción solo si se cumplen varias condiciones al mismo tiempo.

### Condiciones Anidadas

Las condiciones anidadas ocurren cuando una declaración `if` o `switch` se encuentra dentro de otra. Esto es útil cuando se tomaran una serie de decisiones que dependen del resultado de una decisión anterior. Sin embargo, deben usarse con precaución para evitar la complejidad excesiva y mantener la legibilidad del código.

Un ejemplo de condiciones anidadas es:

```javascript
if (condicionExterna) {
  if (condicionInterna) {
    // El código se ejecuta si se cumplen tanto condicionExterna como condicionInterna
  }
}
```

Aunque poderosas, las condiciones anidadas pueden llevar a lo que se conoce como el "problema del triángulo de la muerte" si se abusa de ellas, donde el código se desplaza hacia la derecha y se vuelve difícil de seguir. Una alternativa es usar guard clauses o retornar temprano para mantener el código limpio y plano.

### Triangulo de la muerte

El "problema del triángulo de la muerte" es una forma coloquial de referirse a un patrón de codificación problemático en el que se anidan múltiples estructuras de control, como condicionales `if` o bucles `for`. A medida que se añaden más niveles de anidación, el código se desplaza hacia la derecha, creando una estructura en forma de triángulo que es difícil de leer y mantener. 

### Clausulas de guarda
Las cláusulas de guarda, también conocidas como guard clauses, son una técnica de programación utilizada para mejorar la legibilidad del código al manejar casos de error o condiciones particulares al principio de una función o bloque de código. Este enfoque ayuda a evitar el anidamiento profundo y hace que el código sea más claro y más fácil de seguir.

En lugar de envolver la lógica principal de una función dentro de una estructura condicional, las guard clauses se encargan de los casos especiales o de error al inicio, y si alguna de estas condiciones se cumple, la función termina prematuramente, a menudo con un `return`, `continue`, `break`, o incluso lanzando un error.

Ejemplo:

```javascript
function procesarUsuario(usuario) {
  // Guard clause para un parámetro no definido
  if (!usuario) {
    console.error('El usuario no está definido.');
    return;
  }

  // Guard clause para una propiedad específica
  if (usuario.estado === 'inactivo') {
    console.error('El usuario está inactivo.');
    return;
  }

  // La lógica principal de la función se lleva a cabo si no se activaron las guardias anteriores
  console.log('Procesando usuario:', usuario.nombre);
}
```

Utilizar cláusulas de guarda puede hacer que el código sea más fácil de entender y de mantener, ya que reduce la complejidad que introducen las condiciones anidadas y pone de manifiesto los casos "excepcionales" o importantes al principio del bloque de código.

## Referencias
- [MDN Web Docs - if...else](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Statements/if...else)

- [MDN Web Docs - switch](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Statements/switch)

- [MDN Web Docs - Expressions and operators](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Expressions_and_Operators)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/04-estructuras-de-control/condicionales.md)

[🏡 Volver al inicio](../../readme.md)
