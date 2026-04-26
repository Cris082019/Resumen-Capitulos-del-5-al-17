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

🔵***Dual Stack:*** El equipo habla ambos idiomas a la vez.<br>
🔵***Tunelización:*** Meter paquetes IPv6 dentro de paquetes IPv4.<br>
🔵***Traducción (NAT64):*** Traducir de un protocolo a otro para que se entiendan.

**3. Formato y Reglas de Compresión**<br>
Las direcciones IPv6 son largas (8 grupos de 4 dígitos hexadecimales), pero se pueden acortar con dos reglas:

🔵***Omitir ceros a la izquierda:*** 01ab → 1ab.<br>
🔵***Doble dos puntos (::):*** Reemplaza una secuencia de grupos de ceros. Ojo: Solo se puede usar una vez por dirección.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/96d99411-a0aa-48e1-8979-971a3291aba0" />

## **Capitulo 10**

**1. Direccionamiento Estático vs. Dinámico**<br>
***Asignación Estática:*** El administrador de red configura manualmente la dirección IPv4, la máscara de subred y la puerta de enlace en cada dispositivo. Aunque ofrece un control total sobre los recursos, es un proceso lento en redes grandes y requiere llevar un registro riguroso para evitar duplicados.

***Asignación Dinámica (DHCP):*** Es el método preferido para redes grandes. Automatiza la entrega de direcciones, reduce la carga de trabajo del personal técnico y elimina errores humanos de transcripción.

**2. Funcionamiento de DHCP (Protocolo de Configuración Dinámica de Host)**<br>
***Arrendamiento:*** Las direcciones no se entregan de forma permanente, sino que se "alquilan" por un tiempo determinado. Si un dispositivo se desconecta, su dirección regresa al "pool" (reserva) para ser reutilizada por otro.

➖**El Proceso de Comunicación:**<br>
🔵***DHCP Discover:*** El cliente envía un mensaje de difusión (broadcast) buscando un servidor.<br>
🔵***DHCP Offer:*** El servidor responde ofreciendo una dirección IPv4 disponible.<br>
🔵***DHCP Request:*** El cliente solicita formalmente usar la dirección ofrecida.<br>
🔵***DHCP Acknowledgement:*** El servidor confirma la recepción y finaliza la configuración.

**3. DHCP en Entornos Domésticos y Pequeñas Empresas**<br>
***El Router Inalámbrico:*** Generalmente cumple una doble función: actúa como cliente DHCP para recibir una dirección de Internet del ISP y como servidor DHCP para asignar direcciones a los dispositivos de la casa.

***Configuración Predeterminada:*** La mayoría de estos routers traen el servicio habilitado de fábrica, comúnmente usando la dirección 192.168.0.1 con una máscara 255.255.255.0, la cual sirve como puerta de enlace para toda la red local.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/72c3685b-c045-47f7-b7a1-6af255cc0ea4" />

## **Capitulo 11**

**1. El Router como Límite de la Red**<br>
El enrutador (router) inalámbrico actúa como la frontera física y lógica entre la red local interna y la red de Internet externa.
Puerta de Enlace (Default Gateway): Es la dirección IPv4 de la interfaz del router conectada a la red local. Todos los hosts deben conocerla para enviar datos fuera de su propia red.

➖**Doble rol del Router:**<br>
  🟢***Servidor DHCP:*** Asigna direcciones IP automáticamente a los dispositivos internos (laptops, celulares, etc.).<br>
  🟢***Cliente DHCP:*** Solicita una dirección IP pública al Proveedor de Servicios de Internet (ISP) para poder navegar.

**2. Funcionamiento de NAT (Traducción de Direcciones de Red)**<br>
Dado que los dispositivos internos usan direcciones privadas (no válidas en Internet), el router realiza un proceso de traducción para permitir la comunicación global.

🟢***Traducción de Origen:*** Cuando un paquete sale hacia Internet, el router reemplaza la IP privada del host por su propia IP pública.<br>
🟢***Traducción Inversa:*** Cuando llega una respuesta desde Internet, el router traduce la IP pública de vuelta a la IP privada del host correspondiente.<br>
🟢***Eficiencia:*** La tecnología NAT permite que múltiples dispositivos internos compartan una única dirección IP pública simultáneamente.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/ac2f8bbf-7f7c-4be8-908c-894d1b23b89e" />

## **Capitulo 12**

**1. Direcciones MAC e IP**<br>
Un dispositivo en una red local Ethernet utiliza dos direcciones principales para comunicarse:

🟢***Dirección Física (MAC):*** Se usa para la comunicación directa entre tarjetas de red (NIC) dentro de la misma red local.<br>
🟢***Dirección Lógica (IP):*** Se utiliza para enviar paquetes desde el origen hasta el destino final, ya sea que este se encuentre en la misma red o en una red remota.

**2. Comunicación en Redes Remotas**<br>
Cuando el destino está fuera de la red local:

➖El host de origen envía el paquete a su puerta de enlace predeterminada (la interfaz del router).<br>
➖La dirección MAC de destino en la trama de Ethernet será la del router, no la del host final.<br>
➖El router desencapsula la trama, revisa la IP de destino para determinar la mejor ruta y vuelve a encapsular el paquete en una nueva trama adecuada para el siguiente tramo del camino.

**3. El Dominio de Difusión (Broadcast)**<br>
Un mensaje de difusión es aquel que se envía a todos los hosts de una red local. Su dirección MAC de destino es siempre FFFF.FFFF.FFFF.

Los conmutadores (switches) reenvían estos mensajes a todos sus puertos. El área que abarca estos mensajes se llama dominio de difusión.
Si hay demasiados hosts en un mismo dominio, el tráfico puede ser excesivo y afectar el rendimiento. Para solucionar esto, se utilizan routers para dividir una red grande en varios dominios de difusión más pequeños.

**4. Protocolo ARP (Address Resolution Protocol)**<br>
Cuando un host conoce la IP de destino pero no su dirección MAC, utiliza el proceso ARP (en IPv4) que consta de tres pasos:

🟢***Solicitud:*** El emisor envía una trama de difusión con la IP que busca.<br>
🟢***Respuesta:*** El host que tiene esa dirección IP responde enviando su dirección MAC al emisor.<br>
🟢***Almacenamiento:*** El emisor guarda la relación entre esa IP y esa MAC en una tabla ARP para futuras comunicaciones.<br>
<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/d72ee2c4-2b1d-413e-99ea-0070c0dc5c35" />

## **Capitulo 13**

**1. La Necesidad del Enrutamiento**<br>
A medida que las redes crecen, es fundamental dividirlas para mejorar el rendimiento y la administración. Los criterios principales para segmentar redes son:

🔴***Contención de difusión:*** Evitar que el tráfico de "broadcast" sature toda la red, limitándolo a secciones locales.<br>
🔴***Seguridad:*** Separar grupos de computadoras con información sensible.<br>
🔴***Ubicaciones físicas:*** Interconectar sedes que están geográficamente distantes.<br>
🔴***Agrupación lógica:*** Organizar a los usuarios por departamentos (ej. Contabilidad, Ventas) con necesidades comunes.

**2. El Rol del Enrutador (Router)**<br>
El enrutador es el dispositivo central de la Capa 3 (Capa de Red). Sus funciones principales incluyen:

🔴***Conexión de redes:*** Une diferentes redes IP independientes.<br>
🔴***Toma de decisiones:*** A diferencia de los switches (que usan direcciones MAC de Capa 2), los routers deciden hacia dónde enviar los datos basándose en las direcciones IP de destino.<br>
🔴***Intervención necesaria:*** Siempre que el host de origen y el de destino están en redes diferentes, es obligatorio el uso de un enrutador.

**3. Funcionamiento de la Tabla de Enrutamiento**<br>
Para saber qué camino seguir, el router utiliza una tabla de enrutamiento:

🔴***Proceso de reenvío:*** Al recibir una trama, el router extrae el paquete IP, busca la red de destino en su tabla y lo encapsula en una nueva trama para enviarlo por la interfaz correcta.<br>
🔴***Próximo salto:*** El paquete puede ir directamente al host final o a otro router intermedio (utilizando direcciones MAC obtenidas mediante ARP).<br>
🔴***Actualización de la tabla:*** Las rutas pueden ser ingresadas de forma manual (estáticas) por un administrador o de forma dinámica mediante protocolos de red.

**4. Conceptos de LAN y Puerta de Enlace**<br>
🔴***Definición de LAN:*** Redes bajo el mismo control administrativo que suelen usar Ethernet o Wi-Fi con altas velocidades.<br>
🔴***Dominio de difusión:*** En una única LAN, todos los hosts pueden "verse" directamente mediante ARP. Al dividir la LAN, se reduce el impacto del tráfico, pero se añade complejidad y algo de latencia.<br>
🔴***Gateway (Puerta de enlace):*** Es la dirección IP de la interfaz del router conectada a la red local. Es el punto de salida obligatorio para cualquier mensaje que vaya dirigido a una red externa.<br>

<img width="545" height="367" alt="image" src="https://github.com/user-attachments/assets/05b98fe1-43be-4f83-826a-5214619b1541" />
