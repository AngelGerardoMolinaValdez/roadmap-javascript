# Operadores Aritméticos en JavaScript 👩‍💻
Los operadores aritméticos son caracteres que tienen una función especial al ser relacionado con un tipo de dato(operando). Los operadores aritméticos son utilizados para realizar operaciones matemáticas entre valores numéricos.

## ¿Qué es un operando?
Los operandos son los valores con los que trabajan los operadores. En una operación matemática o en una expresión, los operandos son los números o las variables que se están manipulando, mientras que el operador es la acción que se lleva a cabo sobre ellos.

Por ejemplo, en la expresión matemática `5 + 3`, `5` y `3` son los operandos, y `+` es el operador. En esta expresión, el operador de adición (`+`) está actuando sobre los operandos `5` y `3` para sumarlos.

## Operadores Unarios
Los operadores unarios operan sobre un solo operando. Es decir, aplican un cambio sin un segundo dato en la operación. Ejemplo:

1. **Operador de Negación (`-`)**: Cambia el signo del operando.
    ```javascript
    let a = 5;
    let b = -a;  // b será -5
    ```

2. **Operador de Incremento (`++`)**: Incrementa el valor del operando en 1.
    ```javascript
    let a = 5;
    a++;  // a será 6
    ```

3. **Operador de Decremento (`--`)**: Decrementa el valor del operando en 1.
    ```javascript
    let a = 5;
    a--;  // a será 4
    ```

4. **Operador de Negación Lógica (`!`)**: Invierte el valor booleano del operando.
    ```javascript
    let a = true;
    let b = !a;  // b será false
    ```

5. **Operador typeof**: Devuelve una cadena que indica el tipo de datos del operando.
    ```javascript
    let a = 5;
    console.log(typeof a);  // Imprime 'number'
    ```

6. **Operador delete**: Elimina una propiedad de un objeto.
    ```javascript
    let obj = {a: 5};
    delete obj.a;  // Elimina la propiedad a de obj
    ```

## Operadores Binarios
Los operadores binarios operan sobre dos operandos. Ejemplo:

1. **Operador de Adición (`+`)**: Suma dos operandos.
    ```javascript
    let suma = 5 + 3;  // suma será 8
    ```

2. **Operador de Sustracción (`-`)**: Resta el operando de la derecha del operando de la izquierda.
    ```javascript
    let resta = 10 - 3;  // resta será 7
    ```

3. **Operador de Multiplicación (`*`)**: Multiplica dos operandos.
    ```javascript
    let producto = 4 * 7;  // producto será 28
    ```

4. **Operador de División (`/`)**: Divide el operando de la izquierda por el operando de la derecha.
    ```javascript
    let cociente = 20 / 4;  // cociente será 5
    ```

5. **Operador de Módulo (`%`)**: Devuelve el residuo de la división de los operandos.
    ```javascript
    let residuo = 10 % 3;  // residuo será 1
    ```

6. **Operador de Exponenciación (`**`)**: Eleva el operando de la izquierda a la potencia del operando de la derecha.
    ```javascript
    let potencia = 2 ** 3;  // potencia será 8
    ```

7. **Operadores de Comparación**: Como `==`, `!=`, `===`, `!==`, `<`, `>`, `<=`, `>=`.
    ```javascript
    let a = 5;
    let b = 10;
    console.log(a < b);  // Imprime true
    ```

## Referencias
[developer.mozilla.org - Incremento y decremento](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Operators#incremento_y_decremento)

[developer.mozilla.org - Unarios](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Operators#operadores_unarios)

[developer.mozilla.org - Binarios](https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Operators#operadores_aritméticos)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/03-operadores/operadores-aritmeticos.md)

[🏡 Volver al inicio](../../readme.md)