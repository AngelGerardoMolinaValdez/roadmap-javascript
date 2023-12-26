# Parámetros y Argumentos 🏆

1. **Verdadero o Falso:**
   - "En JavaScript, los parámetros de una función siempre deben ser proporcionados cuando se llama a la función."
   - Verdadero / Falso

2. **Relación de Conceptos:**
   - Relaciona cada término (izquierda) con su descripción correcta (derecha).
     - a. Parámetros Rest
     - b. Parámetros por Defecto
     - c. Desestructuración en Parámetros
     - d. Paso de Argumentos
     - e. Parámetros Obligatorios
     - 1. Extraer propiedades de objetos en la definición de la función.
     - 2. Variables necesarias para ejecutar la función.
     - 3. Agrupar un número indefinido de argumentos en un arreglo.
     - 4. Asignar valores iniciales a los parámetros.
     - 5. Forma en que se transmite información a la función.

3. **Respuesta Libre:**
   - Explica cómo se manejan los objetos y los arreglos cuando se pasan como argumentos a una función en JavaScript.

4. **Identificación de Parámetros Obligatorios:**
   ¿Cuál de los siguientes es un ejemplo de un parámetro obligatorio en una función JavaScript?
   a) `function saludar(nombre = "Invitado") {}`
   b) `function sumar(...numeros) {}`
   c) `function iniciarSesion(usuario, contraseña) {}`

5. **Parámetros Rest (Respuesta Múltiple):**
   ¿Cuáles son las características de los parámetros rest en JavaScript? Elige todas las opciones correctas.
   a) Permiten a una función aceptar un número ilimitado de argumentos.
   b) Deben ser el primer parámetro en la definición de la función.
   c) Se representan usando tres puntos (`...`).
   d) Siempre crean un arreglo con los argumentos recibidos.

6. **Uso de Parámetros por Defecto (Relación de Conceptos):**
   Relaciona los siguientes ejemplos de funciones con sus descripciones:
   - Ejemplos:
     1) `function calcularArea(largo, ancho = 5) {}`
     2) `function unirNombres(primerNombre, segundoNombre = "Pérez") {}`
   - Descripciones:
     a) La función asigna "Pérez" como segundo nombre si no se proporciona.
     b) La función usa 5 como ancho predeterminado si no se especifica.

7. **Desestructuración en Parámetros (Respuesta Libre):**
   Describe cómo funciona la desestructuración en los parámetros de una función y proporciona un ejemplo.

8. **Paso de Objetos como Argumentos (Ejercicio Práctico):**
   Dado el siguiente código, ¿cuál será la salida en la consola?
    ```javascript
    function modificarObjeto(obj) {
     obj.nombre = "NuevoNombre";
    }
    let miObjeto = { nombre: "NombreOriginal" };
    modificarObjeto(miObjeto);
    console.log(miObjeto.nombre);
    ```

---

### [Ir al contenido 📝](../../temario/05-funciones/parametros-argumentos.md)

### [Ir al temario 🔍](../../readme.md)
