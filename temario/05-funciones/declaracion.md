# Declaración de Funciones 👩‍💻

La declaración de función es la forma de crear un bloque de código.

La sintaxis básica es la siguiente:

```javascript
function nombreDeLaFuncion(parametro1, parametro2, ... parametroN) {
    // Cuerpo de la función
}
```

- **nombreDeLaFuncion**: Es el nombre único que identifica la función.
- **parametros**: Lista de parámetros nombrados que la función recibirá. Son opcionales; una función puede no tener parámetros.
- **Cuerpo de la función**: Bloque de código que se ejecutará cuando se llame a la función.

**Ejemplo:**

```javascript
function saludar(nombre) {
    return `Hola, ${nombre}!`;
}

console.log(saludar("Alice")); // Salida: Hola, Alice!
```

En este ejemplo, `saludar` es una función que toma un parámetro (`nombre`) y devuelve un saludo personalizado.

## Funciones Nombradas y Anónimas

### Funciones Nombradas

Una función nombrada tiene un nombre identificador. Esto facilita su llamada desde otras partes del código y también mejora la legibilidad y el manejo de errores.

**Ejemplo de Función Nombrada:**

```javascript
function calcularAreaCuadrado(lado) {
    return lado * lado;
}
```

### Funciones Anónimas

Una función anónima no tiene un nombre identificador. Son útiles en contextos donde la función se utiliza inmediatamente o se pasa como argumento a otra función.

**Ejemplo de Función Anónima:**

```javascript
setTimeout(function() {
    console.log("¡Hola después de 3 segundos!");
}, 3000);
```

Aquí, la función que se pasa a `setTimeout` es anónima; no tiene nombre y se ejecuta después de un retraso.

## Contextos de Uso

- **Definición Directa de Funciones**: Cuando sabes que la función se utilizará en varias ocasiones en el programa.
- **Callbacks**: Funciones anónimas son comúnmente usadas como callbacks, que son funciones pasadas como argumentos a otras funciones y ejecutadas más tarde.

## Consideraciones

- **Hoisting**: Las declaraciones de funciones son "elevadas" (hoisted) a la parte superior de su contexto de ejecución, lo que significa que puedes llamar a una función antes de su declaración en el código.

- **Scope**: El alcance de una función define dónde están disponibles sus variables y parámetros.

- **Recursión**: Una función puede llamarse a sí misma. Sin embargo, es importante tener una condición de salida para evitar un bucle infinito.

- **Diferencia entre argumentos y parámetros**: Los parámetros se definen al crear la función y los argumentos son cuando se invoca la función y se pasan esos datos.

## Referencias
- [Funciones y Clases en MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Functions)

- [Declaraciones de Funciones en MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Statements/function)

- [Funciones Anónimas en MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Functions#Funciones_an%C3%B3nimas)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/05-funciones/declaracion.md)

[🏡 Volver al inicio](../../readme.md)
