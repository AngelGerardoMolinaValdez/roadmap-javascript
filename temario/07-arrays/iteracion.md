# Iteración sobre Arrays 📚

JavaScript proporciona varias maneras de iterar sobre arrays, incluyendo los bucles `for` tradicionales y el bucle `for..of` introducido en ES6 (ECMAScript 2015), que simplifica la iteración sobre elementos de un array.

### Bucle `for` Tradicional

El bucle `for` ha sido la manera clásica de iterar sobre los elementos de un array desde las primeras versiones de JavaScript. Te permite especificar explícitamente tanto la variable de inicio, la condición de parada, como la actualización de la variable en cada iteración.

#### Ejemplo de Uso:

```javascript
const frutas = ["manzana", "banana", "cereza"];
for (let i = 0; i < frutas.length; i++) {
    console.log(frutas[i]);
}
```

### Bucle `for..of`

El bucle `for..of` permite iterar sobre los valores de los elementos iterables (incluyendo arrays, mapas, conjuntos, argumentos, etc.) de una manera más concisa y legible. No necesitas mantener un contador ni acceder a los elementos mediante índices.

#### Ejemplo de Uso:

```javascript
const frutas = ["manzana", "banana", "cereza"];
for (const fruta of frutas) {
    console.log(fruta);
}
```

### Comparación y Cuándo Usar

- **Bucle `for` Tradicional:**
  - Proporciona un control más granular sobre el proceso de iteración.
  - Útil cuando necesitas acceder al índice del elemento durante la iteración o modificar el contador de manera no lineal.

- **Bucle `for..of`:**
  - Más limpio y fácil de leer, especialmente cuando no necesitas el índice del elemento.
  - No es adecuado para casos donde necesitas modificar el array durante la iteración, ya que está diseñado para iterar sobre los valores de los elementos.

## Referencias

- [for - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)
- [for...of - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...of)

---

### [Ir al cuestionario 📝](../../cuestionarios/07-arrays/iteracion.md)

### [Ir al temario 🔍](../../readme.md)
