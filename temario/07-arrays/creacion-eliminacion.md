# Creación y Manipulación de Arrays 📚

Los arrays son objetos utilizados para almacenar múltiples valores en una única variable. Proporcionan una manera de agrupar datos que pertenecen juntos y ofrecen métodos y propiedades para trabajar con estos datos de manera eficiente.

### Creación de Arrays

Hay diferentes formas de crear arrays:

#### Usando el Constructor de Array

```javascript
let miArray = new Array('Elemento1', 'Elemento2', 'Elemento3');
```

#### Usando la Notación de Corchetes

```javascript
let miArray = ['Elemento1', 'Elemento2', 'Elemento3'];
```

### Manipulación de Arrays

Una vez creado un array, hay una variedad de métodos para manipular sus elementos, incluyendo agregar, eliminar y modificar elementos.

#### Agregar Elementos

- **push()** - Añade uno o más elementos al final de un array.
  
```javascript
miArray.push('Elemento4'); // Añade 'Elemento4' al final
```

- **unshift()** - Añade uno o más elementos al inicio de un array.
  
```javascript
miArray.unshift('Elemento0'); // Añade 'Elemento0' al inicio
```

#### Eliminar Elementos

- **pop()** - Elimina el último elemento de un array y lo devuelve.
  
```javascript
let elementoEliminado = miArray.pop(); // Elimina 'Elemento4'
```

- **shift()** - Elimina el primer elemento de un array y lo devuelve.
  
```javascript
let primerElementoEliminado = miArray.shift(); // Elimina 'Elemento0'
```

#### Modificar Elementos

- **splice()** - Se utiliza para añadir, eliminar y reemplazar elementos de un array.
  
```javascript
miArray.splice(1, 0, 'NuevoElemento'); // Añade 'NuevoElemento' en la posición 1
```

#### Acceso y Búsqueda

- **indexOf()** / **lastIndexOf()** - Busca en el array y devuelve la primera/última posición del elemento especificado.
- **find()** / **findIndex()** - Encuentra el primer elemento/índice que cumple una función de prueba.

### Iteración sobre Arrays

JavaScript proporciona varios métodos para iterar sobre arrays, como `forEach()`, `map()`, `filter()`, `reduce()`, y más, permitiendo realizar operaciones sobre cada elemento del array de manera eficiente.

## Referencias

- [Array - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- [Array.prototype.pop() - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop)
- [Array.prototype.shift() - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/shift)
- [Array.prototype.splice() - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)
- [delete operator - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/delete)

---

### [Ir al cuestionario 📝](../../cuestionarios/07-arrays/creacion-eliminacion.md)

### [Ir al temario 🔍](../../readme.md)