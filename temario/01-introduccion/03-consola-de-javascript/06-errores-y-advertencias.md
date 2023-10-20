# Errores y advertencias en JavaScript 👩‍💻
En JavaScript, el objeto `console` proporciona varios métodos para registrar y manejar errores y advertencias, lo que es crucial para la depuración y el monitoreo del comportamiento de una aplicación.

## Métodos Principales
`console.error()`: Utilizado para registrar errores en la consola.
`console.warn()`: Utilizado para registrar advertencias en la consola.
Ejemplo:
```javascript
console.error('Este es un error');
console.warn('Esta es una advertencia');
```

## Propósito
Ayudan a identificar y resolver problemas en el código.

## Visualización
Los errores y advertencias se muestran con iconos y colores distintivos en la consola para diferenciarlos.

## Buena Práctica
Utilizar `console.error()` para registrar errores reales o potenciales que requieren atención.
Utilizar `console.warn()` para registrar condiciones inusuales que no son errores pero podrían indicar un problema.

## Información Adicional
Es posible incluir información adicional en los mensajes de error y advertencia, como el nombre del archivo, el número de línea y el stack trace, para facilitar la depuración.

## Desactivación en Producción
Similar a los logs normales, es una buena práctica desactivar o minimizar los mensajes de error y advertencia en la versión de producción para mejorar el rendimiento y la seguridad.

## Referencias

[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/API/console#:~:text=%23%20%E3%80%900%E2%80%A0console%20,API%20differently%20than%20the%20browsers)

[⏪ Ir al cuestionario](../../../cuestionarios/01-introduccion/03-consola-de-javascript/06-errores-y-advertencias.md)

[🏡 Volver al inicio](../../../readme.md)
