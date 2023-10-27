# Operadores de Comparación en JavaScript 👩‍💻

## Definición
Los operadores de comparación son caracteres especiales que se utilizan para
validar los valores entre dos variables con similares tipos de datos o tipos de
datos que sean compatibles de comparar, ejemplo un numero con otro del mismo tipo como int con int, float con float, string con int, bool con int, etc.

## Tipos De Comparación
- **Igualdad (==):** Compara si dos valores son iguales, convirtiendo los tipos de datos si es necesario.
- **Desigualdad (!=):** Compara si dos valores son diferentes, también convierte tipos de datos si es necesario.
- **Igualdad Estricta (===):** Compara si dos valores son iguales, sin convertir los tipos de datos.
- **Desigualdad Estricta (!==):** Compara si dos valores son diferentes, sin convertir los tipos de datos.
- **Menor que (<), Mayor que (>):** Compara si un valor es menor o mayor que otro.
- **Menor o Igual que (<=), Mayor o Igual que (>=):** Incluye la comparación de igualdad junto con menor o mayor que.

## Comparación Estricta
La comparación estricta se refiere a la comparación de dos valores tanto por su tipo de dato como por su valor. Se realiza utilizando el operador de igualdad (`===`) o el operador de desigualdad (`!==`).

1. **Igualdad Estricta (===)**:
    - El operador de igualdad estricta (`===`) compara si dos valores son iguales en tipo y en valor sin realizar ninguna coerción de tipo.
    - Ejemplo:
        ```javascript
        5 === 5;     // true, mismo tipo y mismo valor
        5 === '5';   // false, diferentes tipos aunque el valor numérico es el mismo
        ```

2. **Desigualdad Estricta (!==)**:
    - El operador de desigualdad estricta (`!==`) compara si dos valores son diferentes en tipo o en valor.
    - Ejemplo:
        ```javascript
        5 !== 10;    // true, mismo tipo pero diferentes valores
        5 !== '5';   // true, diferentes tipos aunque el valor numérico es el mismo
        ```

## Comparación Abstracta
Es un tipo de comparación que se realiza utilizando los operadores de igualdad (`==`) y desigualdad (`!=`). Estos operadores comparan dos valores pero antes de hacer la comparación, pueden convertir los valores a un tipo común, proceso conocido como coerción de tipo.

1. **Igualdad Abstracta (`==`)**:
    - El operador de igualdad abstracta (`==`) compara si dos valores son iguales después de la coerción de tipo.
    - Ejemplo:
        ```javascript
        5 == '5';   // true, el string '5' es convertido a número antes de la comparación
        5 == 5;     // true, mismo tipo y mismo valor
        ```

2. **Desigualdad Abstracta (`!=`)**:
    - El operador de desigualdad abstracta (`!=`) compara si dos valores son diferentes después de la coerción de tipo.
    - Ejemplo:
        ```javascript
        5 != '5';   // false, el string '5' es convertido a número antes de la comparación
        5 != 10;    // true, el valor es diferente
        ```

## Referencias
1. [Expresiones y Operadores - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

2. [Comparaciones de Igualdad y Semejanza - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Equality_comparisons_and_sameness)

3. [Igualdad (==) - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Equality)

4. [Operadores de Comparación - JavaScript | MDN](https://www.devdoc.net/javascript/3246_3247.html)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/03-operadores/operadores-comparacion.md)

[🏡 Volver al inicio](../../readme.md)