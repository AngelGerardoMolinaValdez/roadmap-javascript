# Funciones flecha 🚀

Las funciones flecha, introducidas en ES6, son una forma más corta y concisa de escribir expresiones de función. Son útiles para funciones anónimas y tienen algunas características distintivas en comparación con las funciones tradicionales.

## Sintaxis Básica

La sintaxis básica de una función flecha es la siguiente:

```javascript
const miFuncion = (param1, param2) => {
    return param1 + param2;
};
```

Para una sola expresión, puedes omitir las llaves y la palabra clave `return`:

```javascript
const miFuncion = (param1, param2) => param1 + param2;
```

Si solo hay un parámetro, también puedes omitir los paréntesis:

```javascript
const cuadrado = x => x * x;
```

## Características Clave

- **`this` Ligado Léxicamente:** A diferencia de las funciones tradicionales, `this` dentro de una función flecha se refiere al contexto en el que la función fue creada, no al contexto en el que se invoca.

- **No hay Objeto `arguments`:** Las funciones flecha no tienen su propio objeto `arguments`. Sin embargo, puedes acceder a los argumentos de la función con el operador de reposo (rest operator) o parámetros individuales.

- **No Constructoras:** Las funciones flecha no pueden usarse como funciones constructoras y arrojarán un error si se intenta utilizar `new` con ellas.

- **Menos verbosidad:** Ofrecen una sintaxis más limpia y reducida, lo que las hace ideales para operaciones más pequeñas, especialmente como callbacks o funciones en métodos de array como `map`, `filter`, y `reduce`.

## Ejemplos de Uso

### 1. Como Callbacks

```javascript
[1, 2, 3].map(n => n * 2); // [2, 4, 6]
```

### 2. En Métodos de Objeto

```javascript
const obj = {
    id: 42,
    getId: function() {
        return this.id;
    },
    getIdArrow: () => this.id
};
obj.getId(); // 42
obj.getIdArrow(); // undefined (this no está ligado al objeto)
```

## Diferencias entre función flecha y tradicional

### 1. **Sintaxis**

- **Funciones Tradicionales:**
  Tienen una sintaxis más larga y pueden ser declaradas o expresadas.
  ```javascript
  function suma(a, b) {
      return a + b;
  }
  ```

- **Funciones Flecha:**
  Ofrecen una sintaxis más concisa para operaciones breves.
  ```javascript
  const suma = (a, b) => a + b;
  ```

### 2. **`this` Binding**

- **Funciones Tradicionales:**
  El valor de `this` dentro de una función tradicional depende de cómo se llama la función. Puede variar y a menudo requiere enlazar explícitamente el contexto utilizando `.bind()`, `.call()`, o `.apply()`.

- **Funciones Flecha:**
  Capturan el valor de `this` del contexto circundante (donde se declaran), conocido como binding léxico. Esto es particularmente útil en callbacks y métodos donde deseas que `this` se refiera al contexto exterior.

### 3. **Constructor**

- **Funciones Tradicionales:**
  Pueden ser utilizadas como constructores con el operador `new`.

- **Funciones Flecha:**
  No pueden ser utilizadas como constructores. Si intentas hacerlo, JavaScript lanzará un error.

### 4. **Objeto `arguments`**

- **Funciones Tradicionales:**
  Tienen acceso al objeto `arguments`, que es una colección de todos los argumentos pasados a la función.

- **Funciones Flecha:**
  No tienen su propio objeto `arguments`. Si necesitas acceder a todos los argumentos pasados, debes usar parámetros rest.

### 5. **Métodos y Prototype**

- **Funciones Tradicionales:**
  Pueden tener propiedades y un `prototype`, lo que permite añadir métodos.

- **Funciones Flecha:**
  No tienen un `prototype`, lo que significa que no puedes añadir propiedades o métodos a una función flecha.

### 6. **Uso**

- **Funciones Tradicionales:**
  Son más versátiles y adecuadas para un rango más amplio de propósitos, incluyendo métodos de objetos y funciones que requieren el uso de `this` de manera dinámica.

- **Funciones Flecha:**
  Son ideales para casos donde se necesita una función corta y concisa, como en operaciones de array, y cuando quieres evitar el comportamiento dinámico de `this`.

## Referencias

- [Expresiones de Función Flecha - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

- [Sintaxis de las Funciones Flecha - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions#Syntax)

- [Limitaciones de las Funciones Flecha - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions#No_separate_this)

---

### [Ir al cuestionario ⏪](../../cuestionarios/05-funciones/funciones_flecha.md)

### [Volver al inicio 🏡 ](../../readme.md)
