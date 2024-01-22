# Prototipos de Objetos en JavaScript 📚

### Concepto de Prototipo

En JavaScript, cada objeto tiene un **prototipo**, un objeto del que hereda propiedades y métodos. Este concepto permite la reutilización de propiedades y métodos entre objetos.

#### Prototipo de Objeto

- **Definición:** El prototipo de un objeto es otro objeto al que se accede para propiedades y métodos que el objeto original no tiene.
- **Acceso al Prototipo:**
  - A través de la propiedad `__proto__` (no recomendado para uso en producción debido a cuestiones de rendimiento y compatibilidad).
  - Usando `Object.getPrototypeOf()` (forma recomendada).

### Herencia Prototípica

La herencia en JavaScript se maneja a través de prototipos. Cada objeto tiene un enlace a un prototipo, y este prototipo es un objeto de donde hereda métodos y propiedades.

#### Ejemplo de Herencia Prototípica

```javascript
function Persona(nombre) {
    this.nombre = nombre;
}

Persona.prototype.saludar = function() {
    console.log(`Hola, mi nombre es ${this.nombre}`);
};

let persona1 = new Persona("Ana");
persona1.saludar(); // "Hola, mi nombre es Ana"
```

### Modificación y Extensión de Prototipos

Los prototipos pueden ser extendidos y modificados. Esto significa que puedes añadir o cambiar propiedades y métodos de un prototipo, afectando a todos los objetos que lo heredan.

#### Precaución

Modificar prototipos, especialmente de objetos globales como `Object`, `Array`, etc., puede llevar a comportamientos inesperados y es generalmente desaconsejado.

### `Object.create()`

La función `Object.create()` es una forma de crear objetos con un prototipo específico.

```javascript
let prototipo = {
    metodo: function() {
        console.log("Método del prototipo");
    }
};

let objeto = Object.create(prototipo);
objeto.metodo(); // "Método del prototipo"
```

## Referencias

- [Herencia y la cadena de prototipos - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)
- [Object.create() - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/Object/create)

---

### [Ir al cuestionario 📝](../../cuestionarios/06-objetos/prototipos.md)

### [Ir al temario 🔍](../../readme.md)
