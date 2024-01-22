# Creación de Objetos 📚

Un objeto es una colección de propiedades, y una propiedad es una asociación entre un nombre (o clave) y un valor. Un valor de propiedad puede ser una función, en cuyo caso la propiedad se llama método.

### Crear con Literal de Objeto

La forma más sencilla y común de crear objetos en JavaScript es usando la notación de literal de objeto. Esto se hace definiendo un conjunto de pares clave-valor dentro de llaves `{}`.

```javascript
let libro = {
    titulo: "El Hobbit",
    autor: "J.R.R. Tolkien",
    año: 1937
};
```

### Crear Objeto con el Constructor `new Object()`

También puedes crear un objeto usando el constructor `new Object()` y luego agregarle propiedades.

```javascript
let persona = new Object();
persona.nombre = "Ana";
persona.edad = 25;
```

### Crear Objeto con Constructor Funcional

Puedes definir un constructor funcional y luego usar `new` para crear instancias del objeto.

```javascript
function Automovil(marca, modelo) {
    this.marca = marca;
    this.modelo = modelo;
}

let miAuto = new Automovil("Toyota", "Corolla");
```

### Crear Objeto con `Object.create()`

La función `Object.create()` crea un nuevo objeto, utilizando un objeto existente como el prototipo del nuevo objeto.

```javascript
let protoLibro = {
    mostrarTitulo: function() {
        console.log(this.titulo);
    }
};

let miLibro = Object.create(protoLibro);
miLibro.titulo = "1984";
miLibro.mostrarTitulo(); // Muestra "1984"
```

## Referencias 🌐

- [Trabajando con objetos - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Working_with_Objects)
- [Object.create() - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Object/create)

---

### [Ir al cuestionario 📝](../../cuestionarios/06-objetos/creacion.md)

### [Ir al temario 🔍](../../readme.md)
