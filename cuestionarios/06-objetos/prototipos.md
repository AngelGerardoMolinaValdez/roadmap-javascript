# Prototipos de Objetos en JavaScript

1. **Verdadero o Falso:**
   - Todos los objetos en JavaScript heredan propiedades y métodos de un prototipo.
   - La propiedad `__proto__` es la manera recomendada de acceder al prototipo de un objeto.

2. **Relación de Conceptos:**
   - Relaciona cada término con su descripción correcta:
     - A. `Object.create()`
     - B. Constructor Funcional
     - C. Prototipo
     - Opciones:
       1. Un objeto que sirve como un molde para crear otros objetos que heredan sus propiedades y métodos.
       2. Permite crear un nuevo objeto especificando explícitamente el objeto que debería ser su prototipo.
       3. Un patrón para crear objetos y funciones que simulan clases, donde las instancias heredan de un objeto prototipo.

3. **Ejercicio Práctico:**
   - Escribe un constructor `Auto` que tenga una propiedad `modelo` y un método `mostrarModelo` que imprima el modelo del auto. Luego, crea una instancia de `Auto` y llama al método `mostrarModelo`.

4. **Respuesta Libre:**
   - Explica la diferencia entre herencia prototípica y herencia basada en clases como se ve en otros lenguajes de programación.

5. **Opción Múltiple:**
   - ¿Qué método se utiliza para añadir un nuevo método al prototipo de una función constructora?
     - A) `Object.addPrototype()`
     - B) `Object.prototype.newMethod = function() {}`
     - C) `Function.prototype.methodName = function() {}`
     - D) Ninguna de las anteriores

---

### [Ir al contenido 📝](../../temario/06-objetos/prototipos.md)

### [Ir al temario 🔍](../../readme.md)