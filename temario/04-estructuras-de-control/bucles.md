# Bucles en JavaScript 👩‍💻
Los bucles, comúnmente conocidas como "loops", son estructuras de control de programación que permiten repetir una o más líneas de código de manera controlada. Estos bucles son utilizados para realizar tareas que requieren repetición, como procesar elementos de una colección de datos o realizar una acción hasta que se cumpla una condición específica.

## Bucle For

El bucle `for` es una de las estructuras de control utilizadas para iterar sobre una secuencia o colección de elementos.

### Sintaxis detallada del bucle For

El bucle `for` se compone de tres partes opcionales, todas incluidas en paréntesis y separadas por punto y coma:

```javascript
for (inicialización; condición; incremento) {
  // Código a ejecutar en cada iteración
}
```

- **Inicialización**: Aquí se establece el punto de partida del bucle. A menudo se utiliza para crear e inicializar una variable contadora. Esta expresión se ejecuta una sola vez antes de que comience la ejecución del bucle.
  
- **Condición**: Esta es una expresión que se evalúa antes de cada iteración del bucle. Si la condición es verdadera (`true`), el bucle continuará y el bloque de código dentro del bucle se ejecutará. Si la condición es falsa (`false`), el bucle se detendrá.
  
- **Incremento**: Después de cada iteración del bucle, se ejecuta esta expresión. Generalmente se utiliza para actualizar la variable contadora, lo que eventualmente hará que la condición del bucle se evalúe como falsa y el bucle se detenga.

### Ejemplo de un Bucle For

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i); // Imprimirá los números del 0 al 9
}
```

En este ejemplo, `let i = 0` es la inicialización, `i < 10` es la condición y `i++` es el incremento que aumenta el valor de `i` en 1 después de cada iteración.

### Uso Avanzado del Bucle For

- **Bucle For con múltiples variables**: Se puede inicializar y modificar múltiples variables en un bucle `for`.

```javascript
for (let i = 0, j = 10; i < 10; i++, j--) {
  console.log(i, j); // Imprimirá pares de números en orden ascendente y descendente
}
```

- **Bucles anidados**: Se puede usar un bucle `for` dentro de otro bucle `for` para trabajar con estructuras de datos multidimensionales, como matrices.

```javascript
for (let i = 0; i < 5; i++) {
  for (let j = 0; j < 5; j++) {
    console.log(`Posición [${i}][${j}]`);
  }
}
```

- **Etiquetas de bucle**: Se pueden etiquetar los bucles `for` y luego usar la declaración `break` o `continue` con una etiqueta para alterar el comportamiento del bucle.

```javascript
etiquetaBucleExterno:
for (let i = 0; i < 5; i++) {
  for (let j = 0; j < 5; j++) {
    if (i === 2 && j === 2) {
      break etiquetaBucleExterno; // Rompe el bucle externo cuando i y j son ambos 2
    }
    console.log(`Posición [${i}][${j}]`);
  }
}
```

### Consideraciones importantes para for

- Mantener el cuerpo del bucle simple. Si el cuerpo del bucle es complicado, tomar en consideración llamar a una función desde dentro del bucle.
  
- Precaución con las funciones dentro de bucles. Crear funciones fuera del bucle siempre que sea posible para evitar la redefinición en cada iteración.

## Bucle While

El bucle `while` repite un bloque de instrucciones mientras una condición especificada se evalúa como verdadera (`true`). A diferencia del bucle `for`, que es ideal cuando se conoce el número de iteraciones de antemano, un bucle `while` es preferible cuando el número de iteraciones no es conocido y depende de una condición dinámica.

### Sintaxis del Bucle While

La sintaxis de un bucle `while` es:

```javascript
while (condición) {
  // Bloque de código que se ejecuta mientras la condición sea verdadera
}
```

La **condición** puede ser cualquier expresión que JavaScript pueda evaluar como verdadera o falsa. Cada vez que el bucle comienza una nueva iteración, se evalúa la condición. Si la condición es verdadera, el bloque de código dentro del `while` se ejecuta. Si la condición es falsa, el bucle termina y el flujo del programa continúa con la siguiente instrucción después del bucle `while`.

### Ejemplo Básico de While

```javascript
let contador = 0;

while (contador < 5) {
  console.log(contador);
  contador++;
}
```

En este ejemplo, la variable `contador` se incrementa en uno en cada iteración y el bucle continuará hasta que `contador` sea igual a 5.

### Usos Avanzados

- **Bucles con Condiciones Complejas**: Puedes utilizar expresiones lógicas complejas para la condición, permitiendo bucles que respondan a múltiples factores.

```javascript
let contador = 0;
let continuar = true;
let maxIntentos = 5;

// Bucle while con una condición compuesta
while (contador < maxIntentos && continuar) {
  console.log(`Intento número ${contador + 1}`);

  // Realizamos alguna operación que podría cambiar la condición de continuar
  if (algunaCondicion()) {
    continuar = false; // Esto cambiará la condición de continuar
  }

  contador++; // Incrementamos el contador

  // También podríamos tener una condición adicional para detener el bucle
  if (contador === 3 && condicionEspecial()) {
    console.log("Se ha cumplido una condición especial para detener el bucle.");
    break; // Salimos del bucle si se cumple una condición especial
  }
}

function algunaCondicion() {
  // Aquí iría la lógica que determina si se cumple alguna condición
  // Por simplicidad, devolvemos false
  return false;
}

function condicionEspecial() {
  // Aquí iría la lógica que determina si se cumple una condición especial
  // Por simplicidad, devolvemos true
  return true;
}
```

- **Bucles con Múltiples Variables**: Aunque es menos común, un bucle `while` puede manejar múltiples variables en su condición y actualización.

```javascript
let contador1 = 0;
let contador2 = 10;

// Bucle que continúa mientras se cumplan ambas condiciones
while (contador1 < 5 && contador2 > 5) {
  console.log(`Contador1: ${contador1}, Contador2: ${contador2}`);
  
  // Actualizamos ambas variables para cambiar las condiciones en cada iteración
  contador1++;
  contador2--;
}
```

- **While True con Break**: A veces verás un bucle `while` con una condición siempre verdadera (`while (true)`) y una salida controlada por una declaración `break` dentro del bucle. Esto debe usarse con precaución y comprensión clara de la lógica para prevenir bucles infinitos.

```javascript
let contador = 0;

// Bucle infinito que se rompe internamente
while (true) {
  contador++;

  // Condición para romper el bucle
  if (contador === 10) {
    console.log("Se alcanzó el valor de ruptura");
    break; // Salimos del bucle
  }
}
```

### Consideraciones importantes para while

- **Actualización de la Condición**: Es fundamental actualizar la condición dentro del bucle para evitar un bucle infinito. En el ejemplo anterior, `contador++` asegura que eventualmente la condición `contador < 5` se evalúe como falsa.

- **Bucles Infinitos**: Si olvidas actualizar la variable que controla la condición, o la lógica no conduce a que la condición se vuelva falsa, el bucle `while` se ejecutará indefinidamente, lo que puede bloquear o colapsar el navegador o el entorno de ejecución.

- **Bucles Controlados por Eventos**: Los bucles `while` son útiles en situaciones donde el bucle debe ejecutarse hasta que ocurra un evento específico, como la llegada de datos o una entrada del usuario.

## Bucle Do...While

El bucle `do...while` es una estructura de control de bucle que asegura que un bloque de código se ejecute al menos una vez antes de evaluar la condición para la siguiente iteración. Es similar al bucle `while`, con la diferencia clave de que la condición se comprueba después de que se ha ejecutado el bloque de código, no antes.

### Sintaxis del Bucle Do...While

La sintaxis de un bucle `do...while` es:

```javascript
do {
  // Bloque de código a ejecutar
} while (condición);
```

Aquí, el **bloque de código** dentro del `do` se ejecutará sin importar qué, y solo después de su ejecución se evaluará la **condición** dentro del `while`. Si la condición es `true`, el bucle continuará y el bloque de código se ejecutará nuevamente. Si la condición es `false`, el bucle terminará y el flujo de control pasará a la siguiente instrucción después del `do...while`.

### Ejemplo de Do...While

```javascript
let resultado = '';
let i = 0;

do {
  i = i + 1;
  resultado = resultado + i;
} while (i < 5);

console.log(resultado);
// El valor de resultado será "12345" después de la ejecución del bucle
```

En este ejemplo, el bloque de código incrementa el valor de `i` y concatena este valor a la cadena `resultado`. Después de cada concatenación, se verifica la condición `i < 5`. Cuando `i` alcanza 5, la condición se vuelve falsa y el bucle termina.

### Uso Práctico del Bucle Do...While

El bucle `do...while` es útil en situaciones donde se busca que el código se ejecute al menos una vez antes de la comprobación de la condición, por ejemplo:

- Menús interactivos donde al menos una acción debe ocurrir independientemente de la condición.

```javascript
let eleccion;

do {
  eleccion = prompt("Elige una opción: 'jugar', 'guardar', 'salir'");
  switch (eleccion) {
    case 'jugar':
      console.log("Iniciando juego...");
      // Lógica para iniciar el juego
      break;
    case 'guardar':
      console.log("Guardando juego...");
      // Lógica para guardar el juego
      break;
    case 'salir':
      console.log("Saliendo del juego...");
      // Lógica para salir del juego
      break;
    default:
      console.log("Opción no reconocida. Intenta de nuevo.");
  }
} while (eleccion !== 'salir');
```

- Juegos donde un ciclo de juego debe completarse antes de verificar si debe continuar.

```javascript
let juegoTerminado = false;

do {
  console.log("Jugando...");
  // Lógica del juego aquí

  // Al final de cada ciclo de juego, se determina si el juego ha terminado
  juegoTerminado = verificarSiJuegoTerminado(); // Esta debería ser una función que devuelve un booleano

  if (!juegoTerminado) {
    console.log("¡Un ciclo de juego completo! ¿Deseas continuar?");
    // En un entorno real, se pediría confirmación al jugador aquí
  }
} while (!juegoTerminado);

console.log("Gracias por jugar!");

function verificarSiJuegoTerminado() {
  // Lógica para determinar si el juego ha terminado
  // Por simplicidad, devolvemos true para terminar el bucle
  return true;
}
```

- Operaciones de entrada/salida donde necesitas procesar al menos una unidad de datos antes de verificar si hay más.

```javascript
let datosRecibidos;

do {
  datosRecibidos = obtenerDatos(); // Supongamos que esta función obtiene datos para procesar

  console.log("Procesando datos...");
  // Lógica para procesar los datos aquí

  // Supongamos que esta función verifica si hay más datos para procesar
} while (hayMasDatos());

console.log("Todos los datos han sido procesados.");

function obtenerDatos() {
  // Lógica para obtener datos
  // Por simplicidad, devolvemos algún valor de datos
  return "datos";
}

function hayMasDatos() {
  // Lógica para determinar si hay más datos para procesar
  // Por simplicidad, devolvemos false para terminar el bucle
  return false;
}
```

### Diferencias con el Bucle While

Aunque `while` y `do...while` pueden parecer similares, la principal diferencia radica en el momento de la evaluación de la condición:

- En un bucle `while`, la condición se evalúa antes de ejecutar el bloque de código.
- En un bucle `do...while`, el bloque de código se ejecuta antes de evaluar la condición.

### Consideraciones importantes para do while

- **Evita Bucles Infinitos**: Asegúrate de que la condición del bucle eventualmente se vuelva falsa para evitar un bucle infinito.
- **Claridad en la Condición**: La condición debe ser clara y directamente relacionada con el propósito del bucle para evitar la confusión.
- **Actualización de Variables**: Dentro del bucle, las variables que afectan a la condición deben actualizarse adecuadamente para reflejar el progreso del bucle y llevarlo hacia su conclusión.

## Control de flujo en bucles

El control de flujo en bucles se refiere al conjunto de mecanismos que permiten modificar la ejecución secuencial estándar de un bucle en un programa. Estos mecanismos proporcionan la capacidad de interrumpir la iteración actual o todas las iteraciones restantes, y continuar con la ejecución del código fuera del bucle o iniciar la siguiente iteración. En esencia, el control de flujo determina cuándo y cómo se ejecutarán las siguientes instrucciones dentro del contexto de un bucle.

El control de flujo se emplean principalmente dos declaraciones para el control de flujo dentro de bucles: `break` y `continue`.

### Declaración Break

La declaración `break` termina el bucle actual, `switch`, o la etiqueta de declaración a la que se aplica y transfiere el control a la siguiente instrucción, justo después del bucle o switch terminado.

**Uso de Break:**
```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    break; // Termina el bucle cuando i es igual a 5
  }
  console.log(i); // Se imprimirán los números del 0 al 4
}
```

### Declaración Continue

La declaración `continue` termina la iteración actual (en el ciclo en que se encuentra) y continúa con la siguiente iteración del bucle, omitiendo cualquier código que se encuentre entre ella y el final de la iteración del bucle.

**Uso de Continue:**
```javascript
for (let i = 0; i < 10; i++) {
  if (i % 2 === 0) {
    continue; // Omite la iteración actual si i es un número par
  }
  console.log(i); // Se imprimirán solo los números impares
}
```

### Control de Flujo con Etiquetas

JavaScript también permite el uso de etiquetas que, junto con las declaraciones `break` y `continue`, controlan el flujo de ejecución más complejo, particularmente cuando se trabaja con bucles anidados.

**Uso de Etiquetas:**
```javascript
etiquetaExterna: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    if (i === j) {
      continue etiquetaExterna; // Continúa con la próxima iteración del bucle etiquetado como 'etiquetaExterna'
    }
    console.log(`i = ${i}, j = ${j}`);
  }
}
```

## Consideraciones al Usar Bucles

- Evitar bucles infinitos asegurándose de que la condición eventualmente se vuelva falsa.

- Usar `break` para salir de un bucle si se cumple una condición determinada antes de lo previsto.

- Utilizar `continue` para saltar al inicio del bucle y comenzar la siguiente iteración.

## Referencias
- [MDN Web Docs - Loops and iteration](https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Loops_and_iteration)

- [MDN Web Docs - For loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for)

- [MDN Web Docs - While loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/while)

- [MDN Web Docs - Do...While](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/do...while)

- [MDN Web Docs - Break](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/break)

- [MDN Web Docs - Continue](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/continue)

## Cuestionario
[⏪ Ir al cuestionario](../../cuestionarios/04-estructuras-de-control/bucles.md)

[🏡 Volver al inicio](../../readme.md)
