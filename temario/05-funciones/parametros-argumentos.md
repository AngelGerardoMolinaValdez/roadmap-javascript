# Parámetros y Argumentos 📚

### Diferencias

#### Parámetros
   - Los parámetros son las variables que se enumeran como parte de la definición de la función. 
   - Son como placeholders que representan los valores que la función espera recibir cuando se llama. 
   - Por ejemplo, en la función `function suma(a, b)`, `a` y `b` son parámetros. Representan los valores que se pasarán a la función cuando se llame.

#### Argumentos
   - Los argumentos son los valores reales que se pasan a la función cuando se llama.
   - Son los datos concretos que proporcionas a la función para que trabaje con ellos.
   - Por ejemplo, si llamas a la función `suma(5, 3)`, los valores `5` y `3` son los argumentos. Son los valores específicos que se pasan a la función `suma`.

### Parámetros obligatorios
    - Son los parámetros que necesitan ser especificados al invocar una función
   - Ejemplo:
     ```javascript
     function iniciarSesion(url, username, password) {
         doNothing(url, username, password)
     }
     ```

### Parámetros por Defecto
   - Permiten establecer valores iniciales para los parámetros de la función.
   - Ayudan a evitar errores en caso de que no se pasen argumentos o se pasen argumentos indefinidos.
   - Ejemplo:
     ```javascript
     function saludar(nombre = "Invitado") {
         return `Hola, ${nombre}`;
     }
     ```

### Parámetros Rest
   - Utilizan la sintaxis de tres puntos (`...`) para agrupar un número indefinido de argumentos en un arreglo.
   - Facilitan la creación de funciones que aceptan cualquier número de argumentos.
   - Ejemplo:
     ```javascript
     function sumar(...numeros) {
         return numeros.reduce((total, actual) => total + actual, 0);
     }
     ```

### Desestructuración en Parámetros
   - Permite extraer directamente propiedades de objetos o elementos de arreglos pasados como argumentos.
   - Ejemplo:
     ```javascript
     function mostrarPerfil({ nombre, edad, profesion = "No especificado" }) {
         console.log(`Nombre: ${nombre}, Edad: ${edad}, Profesión: ${profesion}`);
     }

     mostrarPerfil({ nombre: "Ana", edad: 28 });
     // Salida: Nombre: Ana, Edad: 28, Profesión: No especificado
     ```

### Paso de Argumentos
   - Los argumentos son los valores reales que se pasan a la función cuando se llama.
   - En JavaScript, los argumentos se pasan por valor para tipos primitivos y por referencia para objetos.
   - Esto significa que la función puede modificar el estado de un objeto pasado como argumento, pero no puede reasignar completamente un argumento primitivo.

---

## Referencias 🌐
- [Funciones en JavaScript - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Defining_functions) - Una visión general de las funciones en JavaScript, incluyendo cómo se definen y utilizan.
- [Parámetros y Retorno de Funciones - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Function_parameters) - Explicación sobre cómo los parámetros son pasados a las funciones y cómo las funciones devuelven valores.
- [Uso de Objetos como Parámetros - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Using_the_arguments_object) - Muestra cómo los cambios en las propiedades de un objeto pasado como parámetro se reflejan fuera de la función.
- [Modificación de Arrays Pasados como Parámetros - MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions#Using_the_arguments_object) - Ejemplo de cómo los cambios en un arreglo pasado como parámetro son visibles fuera de la función.

---

### [Ir al cuestionario 📝](../../cuestionarios/05-funciones/parametros-argumentos.md)

### [Ir al temario 🔍](../../readme.md)
