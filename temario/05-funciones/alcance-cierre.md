# Alcance y Cierre (Scope & Closure) 📚

### Alcance (Scope)

El alcance se refiere al contexto en el que los valores y expresiones son "visibles" o pueden ser referenciados. Si una variable o función no está en el alcance actual, no se puede acceder a ella. Existen principalmente dos tipos de alcance:

- **Alcance Global:** Una variable o función definida en el alcance global está disponible en cualquier parte del código.
  
- **Alcance Local (Función y Bloque):**
  - **Alcance de Función:** Las variables definidas dentro de una función no son accesibles desde fuera de la función. Cada función tiene su propio alcance.
  - **Alcance de Bloque (introducido en ES6):** Las variables definidas dentro de un bloque (por ejemplo, dentro de `{}` en una estructura de control como `if` o `for`) son accesibles solo dentro de ese bloque. Esto es posible con las palabras clave `let` y `const`.

### Cierre (Closure)

Un closure ocurre cuando una función interna tiene acceso al alcance de su función externa. Los closures permiten que una función interna recuerde y acceda a las variables y argumentos de su función externa, incluso después de que la función externa haya terminado de ejecutarse. Esto es posible debido a cómo JavaScript maneja la memoria y el ámbito léxico.

- **Uso Común:** Los closures son útiles en situaciones como:
  - Encapsulamiento y privacidad de datos.
  - Creación de funciones de fábrica y funciones que manipulan otras funciones (como en la programación funcional).

### Ejemplo de Closure
```javascript
function crearSaludo(saludo) {
    return function(nombre) {
        return `${saludo}, ${nombre}`;
    };
}

const saludoHola = crearSaludo("Hola");
console.log(saludoHola("Ana")); // "Hola, Ana"
```

En este ejemplo, `saludoHola` es un closure que tiene acceso al parámetro `saludo` de la función externa `crearSaludo`, incluso después de que `crearSaludo` haya terminado de ejecutarse.

---

## Referencias 🌐

- [Alcance (Scope) en JavaScript - MDN](https://developer.mozilla.org/en-US/docs/Glossary/Scope) - Una explicación del concepto de alcance en JavaScript, incluyendo cómo las variables y funciones son accesibles en diferentes partes del código.
- [Cierres (Closures) en JavaScript - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures) - Detalles sobre qué son los cierres y cómo proporcionan acceso al alcance de una función externa desde una función interna.

---

### [Ir al cuestionario 📝](../../cuestionarios/05-funciones/alcance-cierre.md)

### [Ir al temario 🔍](../../readme.md)
