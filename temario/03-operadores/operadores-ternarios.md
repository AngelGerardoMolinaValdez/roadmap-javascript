# Operadores ternarios en JavaScript 👩‍💻
El operador ternario es una estructura condicional compacta que consiste en una expresión que se evaluará, y, dependiendo de si la evaluación fue positiva o negativa, devolverá una u otra cosa.

En términos simples, es asignar un valor a una variable si una evaluación es true y asigna otra si es false.

La sintaxis es la siguiente:

```javascript
expresión_condicional ? expresion1 : expresion2;
```

- `expresión_condicional`: Esta es la expresión que se evaluará. Si la evaluación resulta ser verdadera, entonces se ejecutará `expresion1`. Si resulta ser falsa, entonces se ejecutará `expresion2`.
- `expresion1`: Esta expresión se ejecutará y se devolverá en caso de que `expresión_condicional` sea verdadera.
- `expresion2`: Esta expresión se ejecutará y se devolverá en caso de que `expresión_condicional` sea falsa.

Este operador se conoce como ternario porque involucra tres operadores: la expresión condicional a evaluar y dos expresiones a ejecutar para el caso positivo o el negativo.

## Ejemplos de Uso

1. **Limitando un valor**:
    ```javascript
    var valor_x_limitado_a_1000 = (x < 1000) ? x : 1000;
    ```
    Este código devolverá el valor de `x` si `x` es un número menor que 1000. En caso contrario, devolverá 1000【145†source】.

2. **Obteniendo el nombre de un día de la semana**:
    ```javascript
    var numeroDeDia = 3;
    var weekDays = ['lunes', 'martes', 'miércoles', 'jueves', 'viernes', 'sábado', 'domingo'];
    var dia = (numeroDeDia < weekDays.length) ? weekDays[numeroDeDia - 1] : 'dia incorrecto';
    console.log(dia);  // Output: miércoles
    ```
    Este código devolverá el nombre del día correspondiente al número dado, y si el número es incorrecto, devolverá 'dia incorrecto'.

## Referencias
- [Operadores - JavaScript | MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Expressions_and_Operators#operadores_condicionales)

- [Operador ternario en Javascript - Desarrolloweb.com](https://desarrolloweb.com/articulos/operador-ternario-javascript.html)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/03-operadores/operadores-ternarios.md)

[🏡 Volver al inicio](../../readme.md)
