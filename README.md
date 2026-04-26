### Resumen Capitulos del 5 al 17

## ***Capitulo 5***

***Principios de Comunicación***<br>
La comunicación efectiva en red entre computadoras no es un proceso aislado, sino el resultado de la interacción armoniosa entre protocolos, estándares y modelos de referencia.

**1. El Rol de los Protocolos**<br>
Los protocolos son las reglas fundamentales que rigen cómo se envían, reciben e interpretan los datos. Para que dos hosts se comuniquen, deben acordar:

***Formato y Estructura:*** Cómo se organiza el mensaje.<br>
***Codificación:*** La conversión de datos en patrones de luz, sonido o impulsos eléctricos según el medio físico.<br>
***Encapsulación:*** El proceso de agregar información de direccionamiento (origen y destino) en un encabezado para identificar a los involucrados.<br>
***Sincronización y Patrones:*** La velocidad de transmisión de los bits y el método de entrega (ya sea esperando una confirmación de recepción o simplemente transmitiendo los datos).

**2. La Importancia de los Estándares**<br>
Para que dispositivos de distintos fabricantes puedan coexistir en una misma red, se utilizan estándares. Estos son reglas universales que aseguran la interoperabilidad. En el ámbito de Internet, estos estándares son desarrollados y mantenidos por organizaciones como la IETF y se documentan formalmente en los RFC (Solicitud de Comentarios).

<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/899b1c0f-5496-4ef5-a2ec-42a6909463e8" /><br><br>

**3. Modelos de Referencia y Capas**<br>
La comunicación se organiza en "pilas de protocolos" divididas en capas independientes, donde cada nivel presta servicios al superior. Existen dos modelos principales:<br>

Modelo TCP/IP: Es el modelo práctico utilizado en Internet. Se divide en cuatro capas: Aplicación (datos de usuario), Transporte (gestión de comunicación), Internet (ruta de datos) y Acceso a la red (hardware).

Modelo OSI: Es un modelo de referencia detallado de 7 capas que sirve para el diseño y la resolución de problemas:

Física: Transmisión de bits por medios físicos.

Enlace de datos: Intercambio de tramas entre dispositivos.

Red: Direccionamiento y determinación de rutas.

Transporte: Segmentación y reensamblaje de la información.

Sesión: Gestión del diálogo entre aplicaciones.

Presentación: Representación y formato de los datos.

Aplicación: Interfaz para los protocolos de proceso a proceso.
