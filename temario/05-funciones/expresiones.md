# Expresiones de Función en JavaScript 👩‍💻

Las expresiones de función son una forma de definir funciones en JavaScript. A diferencia de las declaraciones de función, las expresiones de función se pueden asignar a variables, pasar como argumentos a otras funciones, y más. Son extremadamente versátiles y útiles en muchos patrones de JavaScript.

## Sintaxis Básica

Una expresión de función típicamente se ve así:

```javascript
const miFuncion = function(param1, param2) {
    // Cuerpo de la función
};
```

En este ejemplo, la función es anónima (no tiene nombre) y se asigna a la variable `miFuncion`. Esta variable luego puede ser usada para invocar la función.

## Características

- **Anónimas o Nombradas:** Aunque las expresiones de función son comúnmente anónimas, también pueden ser nombradas. Esto puede ayudar en la depuración y la recursividad.

    ```javascript
    const ejemplo = function miFuncionNombrada() {
        // Cuerpo de la función
    };
    ```

- **No Hoisting:** A diferencia de las declaraciones de función, las expresiones de función no se benefician del hoisting, lo que significa que no se pueden invocar antes de definirlas en el código.

## Uso como Callbacks

Las expresiones de función son frecuentemente utilizadas como callbacks, es decir, funciones que se pasan como argumentos a otras funciones para ser invocadas más tarde.

Ejemplo:

```javascript
const boton = document.getElementById('miBoton');
boton.addEventListener('click', function() {
    alert("Botón clickeado");
});
```

En este ejemplo, la función que se pasa al `addEventListener` es una expresión de función anónima que se activa cuando se hace clic en el botón.

## IIFE (Immediately Invoked Function Expression)

Una IIFE es una expresión de función que se ejecuta inmediatamente después de su definición.

```javascript
(function() {
    console.log("Esta función se invoca inmediatamente después de su definición");
})();
```

## Ventajas

- **Encapsulación:** Las expresiones de función pueden ayudar a encapsular o esconder la lógica, evitando contaminar el ámbito global.
- **Flexibilidad:** Son ideales para usar en patrones de diseño donde la función necesita ser pasada como un argumento o devuelta por otra función.

## Referencias

- [Expresión de Función en JavaScript - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function)
- [Funciones en JavaScript - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
- [Hoisting de Funciones y Variables - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Glossary/Hoisting)
- [Funciones Nombradas en Expresiones de Función - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/function#Named_function_expression)
- [IIFEs (Immediately Invoked Function Expressions) - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Glossary/IIFE)


## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/05-funciones/expresiones.md)

[🏡 Volver al inicio](../../readme.md)
