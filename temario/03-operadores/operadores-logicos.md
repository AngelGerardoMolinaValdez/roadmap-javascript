# Operadores de Comparación en JavaScript 👩‍💻
Los operadores lógicos son símbolos especiales o palabras que conectan dos o más expresiones de manera tal que el resultado de la operación lógica depende del valor de las expresiones originales. Estos operadores son utilizados para realizar operaciones lógicas, y su resultado es siempre un valor booleano: true o false.

## AND (`&&`)
    - Este operador devuelve `true` si y solo si ambos operandos son `true`.
    - Ejemplo:
        ```javascript
        true && true;   // Retorna true
        true && false;  // Retorna false
        false && true;  // Retorna false
        false && false; // Retorna false
        ```

## OR (`||`)
    - Este operador devuelve `true` si al menos uno de los operandos es `true`.
    - Ejemplo:
        ```javascript
        true || true;   // Retorna true
        true || false;  // Retorna true
        false || true;  // Retorna true
        false || false; // Retorna false
        ```

## NOT (`!`)
    - Este operador invierte el valor booleano del operando.
    - Ejemplo:
        ```javascript
        !true;  // Retorna false
        !false; // Retorna true
        ```

## Tablas de Verdad
Las tablas de verdad muestran el resultado de aplicar operadores lógicos a todos los valores posibles de los operandos. Aquí están las tablas de verdad para los operadores lógicos en JavaScript:

- **AND (`&&`)**:
    | A     | B     | A && B |
    |-------|-------|--------|
    | true  | true  | true   |
    | true  | false | false  |
    | false | true  | false  |
    | false | false | false  |

- **OR (`||`)**:
    | A     | B     | A || B |
    |-------|-------|--------|
    | true  | true  | true   |
    | true  | false | true   |
    | false | true  | true   |
    | false | false | false  |

- **NOT (`!`)**:
    | A     | !A    |
    |-------|-------|
    | true  | false |
    | false | true  |

## Referencias
1. [Expresiones y operadores - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

2. [AND Lógico (&&) - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_AND)

3. [OR Lógico (||) - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_OR)

4. [Operadores Lógicos - JavaScript | MDN (DevDoc)](https://www.devdoc.net/javascript/3246_3247.html)

5. [Operadores Lógicos - Tutorial Moderno de JavaScript](https://javascript.info/logical-operators)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/03-operadores/operadores-logicos.md)

[🏡 Volver al inicio](../../readme.md)