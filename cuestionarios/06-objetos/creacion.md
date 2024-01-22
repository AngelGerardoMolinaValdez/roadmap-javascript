# Creación de Objetos 🏆

1. **Verdadero o Falso:** 
   - Un objeto en JavaScript no puede contener funciones como propiedades.

2. **Relación de Conceptos:** 
   - Relaciona cada método de creación de objetos con su descripción adecuada:
     - A. Literal de objeto
     - B. Constructor `new Object()`
     - C. Constructor Funcional
     - D. `Object.create()`
     - Opciones: 
       1. Crea un objeto nuevo usando un objeto existente como prototipo.
       2. Utiliza la notación de llaves `{}` para definir pares clave-valor.
       3. Crea un objeto y luego se le agregan propiedades individualmente.
       4. Define una función que asigna propiedades a través de `this`, y luego se usa `new` para instanciar.

3. **Ejercicio Práctico:**
   - Escribe una función constructora `Persona` que cree un objeto con propiedades `nombre` y `edad`, y un método `saludar` que imprima "Hola, soy [nombre]".

4. **Respuesta Libre:**
   - ¿Cuáles son las ventajas de usar el literal de objeto frente a `new Object()` para crear objetos?

5. **Opción Múltiple:**
   - ¿Qué muestra `console.log` en el siguiente código?
     ```javascript
     let protoLibro = {
         mostrarTitulo: function() {
             console.log(this.titulo);
         }
     };

     let miLibro = Object.create(protoLibro);
     miLibro.titulo = "1984";
     miLibro.mostrarTitulo();
     ```
     - A) "1984"
     - B) `undefined`
     - C) Un error
     - D) Nada

---

### [Ir al contenido 📝](../../temario/06-objetos/creacion.md)

### [Ir al temario 🔍](../../readme.md)
