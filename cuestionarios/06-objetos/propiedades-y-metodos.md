# Propiedades y Métodos 🏆

1. **Verdadero o Falso:**
   - En JavaScript, las propiedades de los objetos solo pueden ser de tipo string o número.
   - Los métodos de un objeto no pueden hacer referencia a otras propiedades del mismo objeto utilizando `this`.

2. **Relación de Conceptos:**
   - Relaciona cada término con su descripción correcta:
     - A. Getter
     - B. Setter
     - C. Notación de punto
     - D. Notación de corchetes
     - Opciones:
       1. Se utiliza para acceder a una propiedad de un objeto mediante una clave como string.
       2. Método especial para establecer el valor de una propiedad.
       3. Método especial para obtener el valor de una propiedad.
       4. Se utiliza para acceder directamente a una propiedad de un objeto.

3. **Ejercicio Práctico:**
   - Crea un objeto `estudiante` con propiedades `nombre` y `edad`, y un método `presentarse` que imprima "Hola, soy [nombre] y tengo [edad] años".

4. **Respuesta Libre:**
   - ¿Cuál es la diferencia entre usar métodos getters/setters y acceder directamente a las propiedades de un objeto?

5. **Opción Múltiple:**
   - ¿Qué imprime el siguiente código?
     ```javascript
     let objeto = {
         dato: "Valor inicial",
         get obtenerDato() {
             return this.dato;
         },
         set modificarDato(valor) {
             this.dato = valor;
         }
     };

     objeto.modificarDato = "Nuevo valor";
     console.log(objeto.obtenerDato);
     ```
     - A) "Valor inicial"
     - B) "Nuevo valor"
     - C) Un error
     - D) Nada

---

### [Ir al contenido 📝](../../temario/06-objetos/propiedades-y-metodos.md)

### [Ir al temario 🔍](../../readme.md)
