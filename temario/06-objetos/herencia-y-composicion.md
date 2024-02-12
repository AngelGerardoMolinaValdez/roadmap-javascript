# Herencia y Composición 📚

La herencia y la composición son dos conceptos de la programación orientada a objetos que permiten la reutilización de código de diferentes maneras. En JavaScript, estos conceptos se pueden aplicar de manera flexible gracias a su naturaleza dinámica y su sistema de prototipos.

### Herencia

La herencia es un principio por el cual un objeto puede heredar propiedades y métodos de otro objeto. En JavaScript, la herencia se realiza a través de la cadena de prototipos.

- **Herencia Prototípica:**
  Cualquier objeto puede ser el prototipo de otro objeto. Esto permite la creación de una cadena de herencia donde los objetos pueden heredar comportamientos de sus prototipos.

- **Utilizando `Object.create()`:**
  `Object.create()` es un método que crea un nuevo objeto, usando un objeto existente como el prototipo del nuevo objeto creado. Esto permite implementar herencia directa entre objetos.

- **Funciones Constructoras y `prototype`:**
  Las funciones constructoras pueden ser utilizadas para simular clases. Al extender el prototipo de una función constructora, cualquier objeto creado con ella heredará esos métodos y propiedades.

### Composición

La composición es un enfoque donde se combina o compone objetos más simples para construir objetos más complejos. En lugar de heredar todo de un único ancestro (como en la herencia), un objeto compuesto puede obtener funcionalidad y datos de múltiples fuentes.

- **Composición sobre Herencia:**
  En muchos casos, la composición puede ser más flexible y mantenible que la herencia. Permite combinar comportamientos de múltiples objetos sin crear una jerarquía de clases rígida.

- **Ejemplo de Composición:**
  ```javascript
  const hablarMixin = {
      hablar() {
          console.log(`Mi nombre es ${this.nombre}`);
      }
  };

  const caminarMixin = {
      caminar() {
          console.log("Estoy caminando");
      }
  };

  function Persona(nombre) {
      this.nombre = nombre;
  }

  // Componer los comportamientos en Persona
  Object.assign(Persona.prototype, hablarMixin, caminarMixin);

  const juan = new Persona("Juan");
  juan.hablar();
  juan.caminar();
  ```

### Comparación

- **Herencia:**
  - Es útil para crear una relación "es un/a" entre objetos.
  - Puede llevar a jerarquías complejas y frágiles.

- **Composición:**
  - Es útil para una relación "tiene un/a" o "usa un/a".
  - Promueve una mayor flexibilidad y reutilización de código.

## Referencias

- [Composition over inheritance - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain#Composition_over_inheritance)
- [Understanding Prototypes and Inheritance in JavaScript - MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Inheritance)

---

### [Ir al cuestionario 📝](../../cuestionarios/06-objetos/herencia-y-composicion.md)

### [Ir al temario 🔍](../../readme.md)