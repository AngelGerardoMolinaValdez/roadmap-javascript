# Propiedades y Métodos 📚

### Acceso y Modificación de Propiedades

- **Acceso a Propiedades:**
  Se puede acceder a las propiedades de un objeto utilizando la notación de punto o la notación de corchetes.
  ```javascript
  let persona = { nombre: "Ana", edad: 25 };
  console.log(persona.nombre); // Notación de punto
  console.log(persona['edad']); // Notación de corchetes
  ```

- **Modificación de Propiedades:**
  Las propiedades de los objetos pueden ser modificadas o nuevas propiedades pueden ser añadidas en cualquier momento.
  ```javascript
  persona.nombre = "Juan";
  persona['edad'] = 30;
  persona.profesion = "Ingeniero"; // Añadir nueva propiedad
  ```

### Métodos de los Objetos

Los métodos son funciones asociadas a un objeto. Son una forma de agrupar funcionalidades relacionadas con el objeto.

- **Declaración de Métodos:**
  Se pueden declarar dentro del literal de objeto.
  ```javascript
  let persona = {
      nombre: "Ana",
      saludar: function() {
          console.log(`Hola, mi nombre es ${this.nombre}`);
      }
  };
  persona.saludar(); // Llamada al método
  ```

- **Métodos en ES6:**
  Con la sintaxis de ES6, los métodos pueden ser definidos de manera más concisa.
  ```javascript
  let persona = {
      nombre: "Ana",
      saludar() {
          console.log(`Hola, mi nombre es ${this.nombre}`);
      }
  };
  ```

### `this` en Métodos

El valor de `this` dentro de un método hace referencia al objeto al cual el método pertenece. Es importante para acceder a otras propiedades y métodos del mismo objeto.

### Métodos Especiales: Getters y Setters

JavaScript permite definir métodos especiales llamados getters y setters para acceder y modificar las propiedades de un objeto de manera controlada.

- **Getters:** Son métodos que se usan para obtener el valor de una propiedad.
  ```javascript
  let persona = {
      nombre: "Ana",
      get nombreMayus() {
          return this.nombre.toUpperCase();
      }
  };
  console.log(persona.nombreMayus); // ANA
  ```

- **Setters:** Son métodos que se usan para modificar el valor de una propiedad.
  ```javascript
  let persona = {
      nombre: "Ana",
      set cambiarNombre(nuevoNombre) {
          this.nombre = nuevoNombre;
      }
  };
  persona.cambiarNombre = "Elena";
  console.log(persona.nombre); // Elena
  ```

## Referencias 🌐

- [Trabajando con objetos - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Working_with_Objects)
- [Getters y Setters - MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Functions/get)

---

### [Ir al cuestionario 📝](../../cuestionarios/06-objetos/propiedades-y-metodos.md)

### [Ir al temario 🔍](../../readme.md)
