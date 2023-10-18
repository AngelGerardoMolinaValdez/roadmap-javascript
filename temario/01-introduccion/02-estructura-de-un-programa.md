# Estructura de un programa en JavaScript 👩‍💻

La estructura de un programa se refiere a cómo se organiza y se estructura el código. Un buen diseño estructural hace que el código sea más fácil de leer, entender y mantener.

Los componentes de un programa en Javascript se refiere a los siguientes puntos:

## 1. **Declaración de Variables y Constantes**:
   - Las variables y constantes son fundamentales en cualquier programa, y en JavaScript se pueden declarar utilizando las palabras clave `var`, `let` o `const`.
   - Ejemplo:
     ```javascript
     let nombre = "Juan";
     const PI = 3.14159;
     ```

## 2. **Definición de Funciones**:
   - Las funciones son bloques de código reutilizables que se pueden llamar con un nombre específico.
   - Ejemplo:
     ```javascript
     function saludar(nombre) {
       console.log("Hola, " + nombre);
     }
     ```

## 3. **Expresiones y Operadores**:
   - Las expresiones son combinaciones de valores y operadores que pueden ser evaluados.
   - Ejemplo:
     ```javascript
     let resultado = 5 + 10;
     ```

## 4. **Estructuras de Control**:
   - Permiten controlar el flujo del programa mediante condiciones y bucles.
   - Ejemplo:
     ```javascript
     if (resultado > 10) {
       console.log("El resultado es mayor que 10");
     } else {
       console.log("El resultado es menor o igual a 10");
     }
     ```

## 5. **Manipulación del DOM (Document Object Model)**:
   - JavaScript permite interactuar con el DOM para manipular la estructura de una página web en tiempo real.
   - Ejemplo:
     ```javascript
     document.getElementById("miElemento").innerText = "Nuevo Texto";
     ```

## 6. **Eventos**:
   - Los eventos permiten reaccionar a las interacciones del usuario, como clics, ingreso de teclado, entre otros.
   - Ejemplo:
     ```javascript
     document.getElementById("miBoton").addEventListener("click", function() {
       alert("¡Botón presionado!");
     });
     ```

## 7. **Comentarios**:
   - Los comentarios son útiles para explicar el código y hacerlo más legible.
   - Ejemplo:
     ```javascript
     // Esto es un comentario de una línea
     ```

## 8. **Importación y Exportación de Módulos**:
   - Los módulos permiten separar el código en diferentes archivos y importar/exportar funciones, objetos o valores entre ellos.
   - Ejemplo:
     ```javascript
     // archivo.js
     export function miFuncion() { ... }

     // otroArchivo.js
     import { miFuncion } from './archivo.js';
     ```

## Conclusiones

Estos componentes se pueden organizar de diversas maneras para formar un programa completo. Un programa funcional en JavaScript incluirá una mezcla de estos componentes. Estarán organizadas de manera lógica para realizar una tarea específica o resolver un problema particular.

**NOTA:** Todos estos temas los veremos a profundidad en los próximos capítulos

[⏪ Ir al cuestionario](../../cuestionarios/01-introduccion/02-estructura-de-un-programa.md)

[🏡 Volver al inicio](../../readme.md)