### Resumen Capitulos del 5 al 17

## ***Capitulo 5***

***Principios de Comunicación***<br>
La comunicación efectiva en red entre computadoras no es un proceso aislado, sino el resultado de la interacción armoniosa entre protocolos, estándares y modelos de referencia.

**1. El Rol de los Protocolos**<br>
Los protocolos son las reglas fundamentales que rigen cómo se envían, reciben e interpretan los datos. Para que dos hosts se comuniquen, deben acordar:

🔴***Formato y Estructura:*** Cómo se organiza el mensaje.<br>
🔴***Codificación:*** La conversión de datos en patrones de luz, sonido o impulsos eléctricos según el medio físico.<br>
🔴***Encapsulación:*** El proceso de agregar información de direccionamiento (origen y destino) en un encabezado para identificar a los involucrados.<br>
🔴***Sincronización y Patrones:*** La velocidad de transmisión de los bits y el método de entrega (ya sea esperando una confirmación de recepción o simplemente transmitiendo los datos).

**2. La Importancia de los Estándares**<br>
Para que dispositivos de distintos fabricantes puedan coexistir en una misma red, se utilizan estándares. Estos son reglas universales que aseguran la interoperabilidad. En el ámbito de Internet, estos estándares son desarrollados y mantenidos por organizaciones como la IETF y se documentan formalmente en los RFC (Solicitud de Comentarios).<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/899b1c0f-5496-4ef5-a2ec-42a6909463e8" /><br>

**3. Modelos de Referencia y Capas**<br>
La comunicación se organiza en "pilas de protocolos" divididas en capas independientes, donde cada nivel presta servicios al superior. Existen dos modelos principales:<br>

**Modelo TCP/IP:** Es el modelo práctico utilizado en Internet. Se divide en cuatro capas: Aplicación (datos de usuario), Transporte (gestión de comunicación), Internet (ruta de datos) y Acceso a la red (hardware).

**Modelo OSI:** Es un modelo de referencia detallado de 7 capas que sirve para el diseño y la resolución de problemas:

🔴***Física:*** Transmisión de bits por medios físicos.<br>
🔴***Enlace de datos:*** Intercambio de tramas entre dispositivos.<br>
🔴***Red:*** Direccionamiento y determinación de rutas.<br>
🔴***Transporte:*** Segmentación y reensamblaje de la información.<br>
🔴***Sesión:*** Gestión del diálogo entre aplicaciones.<br>
🔴***Presentación:*** Representación y formato de los datos.<br>
🔴***Aplicación:*** Interfaz para los protocolos de proceso a proceso.

## ***Capitulo 6***

**1. Tipos de medios modernos**<br>
Las redes utilizan principalmente tres formas para conectar dispositivos, diferenciándose en cómo codifican los datos:

🔴***Hilos metálicos (cobre):*** Los datos viajan como impulsos eléctricos.<br>
🔴***Fibra de vidrio o plástico (fibra óptica):*** Los datos viajan como pulsos de luz.<br>
🔴***Transmisión inalámbrica:*** Los datos viajan mediante la modulación de ondas electromagnéticas

**2. Criterios para elegir un medio**<br>
Para seleccionar el medio adecuado, se deben considerar cuatro factores:

La distancia máxima que puede alcanzar la señal.<br>
El entorno de instalación.<br>
La cantidad y velocidad de los datos.<br>
El costo de la instalación.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/48886704-1ba0-45f6-9cf0-6f7e4129bb5d" />

## **Capitulo 7**

***1. Encapsulación de Datos***<br>
Es el proceso de envolver un mensaje en un formato específico (como una carta en un sobre) para su transporte. La trama de Ethernet incluye las direcciones MAC (origen/destino), códigos de sincronización y un sistema de verificación para detectar errores de transmisión.

***2. Evolución de la Capa de Acceso***<br>
**Hubs (Concentradores):** Dispositivos obsoletos que permiten solo una comunicación a la vez; generan colisiones y lentitud.<br>
**Switches (Conmutadores):** Dispositivos modernos de Capa 2 que permiten comunicaciones simultáneas, eliminando las colisiones y mejorando el rendimiento.

***3. Inteligencia del Switch***<br>
El switch gestiona la red mediante una tabla de direcciones MAC que construye dinámicamente. Al recibir una trama, "aprende" la ubicación del emisor y busca al destinatario para establecer una conexión directa y temporal entre sus puertos.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/58ac8fcc-394a-49ca-8a7a-c81f1394511b" />

## **Capitulo 8**

**1. Propósito de la Dirección IPv4**<br>
Identificación Lógica: Una dirección IPv4 es una dirección de red lógica que identifica de forma única a un host específico.

🔵***Comunicación Local y Remota:*** Para permitir la comunicación, la dirección debe ser única tanto dentro de una red LAN local como a nivel mundial para conexiones remotas.<br>
🔵***Asignación de Interfaz:*** Se asigna a la conexión de la interfaz de red (NIC) de un dispositivo.<br>
🔵***Enrutamiento de Paquetes:*** Cada paquete enviado por Internet contiene una dirección de origen y una de destino, permitiendo que los dispositivos de red aseguren que la información llegue y las respuestas vuelvan al origen.

**2. Estructura de la Dirección IPv4**<br>
🔵***Composición de 32 bits:*** Tiene una estructura jerárquica de 32 bits dividida en dos partes fundamentales: la porción de red y la porción de host.<br>
🔵***Direccionamiento Jerárquico:*** Esta estructura permite que los enrutadores solo necesiten conocer cómo llegar a cada red en lugar de rastrear cada host individualmente.<br>
🔵***Máscara de Subred:*** Se utiliza para identificar qué octetos corresponden a la red y cuáles al host. Por ejemplo, en la dirección 192.168.5.11 con máscara 255.255.255.0:<br>
192.168.5 identifica la red.<br>
.11 identifica al host específico.<br>
🔵***Redes Lógicas:*** El direccionamiento IPv4 permite la existencia de múltiples redes lógicas dentro de una misma infraestructura física, siempre que las porciones de red sean diferentes.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/c30bda84-7a78-4fad-8235-1d1ae3297ed2" />

## **Capitulo 9**

**1. Problemas con IPv4 y la Migración a IPv6**<br>
IPv4 se quedó sin direcciones. IPv6 soluciona esto con 128 bits, permitiendo un espacio casi infinito (340 sextillones) y mejorando la autoconfiguración y seguridad (ICMPv6).

**2. Métodos de Transición**<br>
Como IPv4 e IPv6 deben convivir, se usan tres técnicas:

***Dual Stack:*** El equipo habla ambos idiomas a la vez.<br>
***Tunelización:*** Meter paquetes IPv6 dentro de paquetes IPv4.<br>
***Traducción (NAT64):*** Traducir de un protocolo a otro para que se entiendan.

**3. Formato y Reglas de Compresión**<br>
Las direcciones IPv6 son largas (8 grupos de 4 dígitos hexadecimales), pero se pueden acortar con dos reglas:

***Omitir ceros a la izquierda:*** 01ab → 1ab.<br>
***Doble dos puntos (::):*** Reemplaza una secuencia de grupos de ceros. Ojo: Solo se puede usar una vez por dirección.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/96d99411-a0aa-48e1-8979-971a3291aba0" />

## **Capitulo 10**

**1. Direccionamiento Estático vs. Dinámico**<br>
***Asignación Estática:*** El administrador de red configura manualmente la dirección IPv4, la máscara de subred y la puerta de enlace en cada dispositivo. Aunque ofrece un control total sobre los recursos, es un proceso lento en redes grandes y requiere llevar un registro riguroso para evitar duplicados.

***Asignación Dinámica (DHCP):*** Es el método preferido para redes grandes. Automatiza la entrega de direcciones, reduce la carga de trabajo del personal técnico y elimina errores humanos de transcripción.

**2. Funcionamiento de DHCP (Protocolo de Configuración Dinámica de Host)**<br>
***Arrendamiento:*** Las direcciones no se entregan de forma permanente, sino que se "alquilan" por un tiempo determinado. Si un dispositivo se desconecta, su dirección regresa al "pool" (reserva) para ser reutilizada por otro.

**El Proceso de Comunicación:**<br>
***DHCP Discover:*** El cliente envía un mensaje de difusión (broadcast) buscando un servidor.<br>
***DHCP Offer:*** El servidor responde ofreciendo una dirección IPv4 disponible.<br>
***DHCP Request:*** El cliente solicita formalmente usar la dirección ofrecida.<br>
***DHCP Acknowledgement:*** El servidor confirma la recepción y finaliza la configuración.

**3. DHCP en Entornos Domésticos y Pequeñas Empresas**<br>
***El Router Inalámbrico:*** Generalmente cumple una doble función: actúa como cliente DHCP para recibir una dirección de Internet del ISP y como servidor DHCP para asignar direcciones a los dispositivos de la casa.

***Configuración Predeterminada:*** La mayoría de estos routers traen el servicio habilitado de fábrica, comúnmente usando la dirección 192.168.0.1 con una máscara 255.255.255.0, la cual sirve como puerta de enlace para toda la red local.
