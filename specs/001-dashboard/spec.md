# Especificación: Dashboard de rendimiento de influencer y afiliación

## Contexto

La influencer promociona productos mediante enlaces y códigos de afiliación en varias redes sociales. Los datos sociales, de campañas y de ventas están repartidos entre plataformas, lo que dificulta comparar resultados y decidir dónde enfocar el contenido.

El dashboard debe reunir esos indicadores en una sola vista orientada a la toma de decisiones. Su interfaz se divide estrictamente en tres bloques visuales: visión ejecutiva, diagnóstico de resultados y operación/alertas.

## Objetivo

Permitir que la influencer comprenda el rendimiento de sus plataformas, productos y campañas durante un período seleccionado, identifique cambios relevantes y priorice oportunidades de mejora sin tener que consultar cada fuente por separado.

## Usuarios

- **Usuaria principal:** influencer o creadora de contenido que gestiona promociones de afiliación.
- **Necesidades:** entender ingresos y conversiones, identificar qué contenido funciona y detectar pronto anomalías que requieren atención.

## Alcance funcional

### Requisitos generales

- **RG-01.** La interfaz debe estar en español y presentar importes en euros con formato local.
- **RG-02.** El dashboard debe organizar todo el contenido en los tres bloques definidos en esta especificación, en ese orden.
- **RG-03.** Debe permitir consultar un período de análisis y mostrar claramente el período activo.
- **RG-04.** Los datos de demostración deben identificarse como simulados. Ninguna métrica debe presentarse como conexión en vivo si no existe una fuente real conectada.
- **RG-05.** La atribución de ventas debe poder asociar la conversión con plataforma, producto y campaña mediante el enlace o código de afiliación correspondiente.

### Bloque superior: KPIs principales

Debe ofrecer una visión ejecutiva con las siguientes métricas:

- **Volumen:** ventas completadas, inscripciones, usuarios activos e impresiones.
- **Ingresos:** comisiones acumuladas y ventas brutas, además del ticket medio de venta.
- **Engagement y rendimiento:** tasa global de engagement, interacciones, CTR y tasa de conversión global.
- **Eficiencia y retorno:** ROI global o por plataforma y coste por resultado.
- Cuando exista comparación temporal, cada KPI debe mostrar el período de comparación y señalar si la variación es positiva, negativa o neutra.

### Bloque intermedio: drivers del resultado

Debe facilitar el diagnóstico de los factores que explican los resultados:

- **Funnel:** alcance → clics en enlaces → ventas completadas, con cantidades y tasas entre etapas.
- **Plataformas:** comparativa de alcance/volumen, conversiones e ingresos por plataforma, incluyendo Instagram, TikTok y YouTube, y permitiendo incorporar otras.
- **Productos:** comparativa de ventas, comisiones generadas y tasa de conversión para los productos A, B y C.
- **Actividad frente a engagement:** cantidad de publicaciones por formato (posts, reels, stories y vídeos) comparada con likes, comentarios, compartidos, guardados u otras interacciones disponibles.

### Bloque inferior: detalle operativo y alertas

Debe incluir:

- **Tabla de productos:** precio, comisión unitaria, conversiones, comisiones generadas y ROI.
- **Tabla de plataformas:** alcance, engagement, conversiones y señalización de la plataforma TOP según el criterio de rendimiento seleccionado.
- **Tabla de campañas:** fechas, producto promocionado, resultados y rendimiento.
- **Alertas automáticas:** detección de caídas relevantes de conversión, picos atípicos y anomalías de rendimiento, con el indicador y período afectados.
- **Listados de control:** TOP Productos, TOP Plataformas, TOP Campañas y Oportunidades de Mejora. Los listados TOP deben poder ordenarse por su métrica de referencia; las oportunidades deben indicar el dato que motiva la recomendación.

## Reglas de negocio y métricas

### Portafolio y comisiones

La comisión fija de cada venta completada es el 15% del precio del producto.

| Producto | Precio | Comisión unitaria | Tasa de comisión |
|---|---:|---:|---:|
| Producto A | 50,00 € | 7,50 € | 15% |
| Producto B | 120,00 € | 18,00 € | 15% |
| Producto C | 80,00 € | 12,00 € | 15% |

### Definiciones

- **Ventas totales:** cantidad de ventas completadas y atribuidas dentro del período. No equivale a ventas brutas.
- **Ventas brutas:** suma del precio de cada producto por sus ventas completadas.
- **Comisiones acumuladas:** suma de la comisión unitaria por las ventas completadas. Las ventas pendientes o canceladas no generan comisión.
- **Ticket medio:** ventas brutas / ventas completadas.
- **CTR:** clics en enlaces / impresiones × 100.
- **Conversión global:** ventas completadas / alcance × 100, según la definición solicitada. Debe distinguirse de la conversión de clic a venta.
- **Conversión de clic a venta:** ventas completadas / clics en enlaces × 100.
- **Engagement global:** interacciones totales / alcance total × 100. El total se calcula con numeradores y denominadores agregados, no mediante el promedio simple de tasas por plataforma.
- **ROI:** ingresos por comisiones / costes atribuibles. Si no hay costes disponibles para la plataforma o campaña, el ROI se debe mostrar como no disponible y no como cero.
- **Coste por resultado:** costes atribuibles / resultados. Para el KPI principal, el resultado es una venta completada; la etiqueta debe indicar la unidad.
- **Plataforma TOP:** la plataforma con mayores comisiones atribuidas en el período, salvo que la usuaria seleccione otro criterio explícito.
- **Tasas agregadas:** se calculan a partir de los totales del período para evitar promediar porcentajes de bases distintas.

### Datos de demostración conocidos

Los siguientes valores describen el prototipo y sirven para comprobar coherencia aritmética. No representan datos conectados a cuentas reales.

- **Volumen:** 847 ventas completadas; 2.341 inscripciones; 12.890 usuarios activos; 456.000 impresiones y 456.000 de alcance simulado.
- **Productos:** A, 412 ventas; B, 198; C, 237. El total por producto es 847 ventas.
- **Ventas brutas:** 63.320 € (20.600 € de A, 23.760 € de B y 18.960 € de C).
- **Comisiones:** 9.498 € (3.090 € de A, 3.564 € de B y 2.844 € de C).
- **Ticket medio:** 63.320 € / 847 = 74,76 €.
- **Plataformas:** Instagram, 412 ventas y 4.620 € en comisiones; TikTok, 287 y 3.230 €; YouTube, 148 y 1.648 €. Los totales coinciden con ventas y comisiones por producto.
- **Clics:** 14.592 en total. Con 456.000 impresiones, el CTR de referencia es 3,2%.
- **Conversión global:** 847 / 456.000 = 0,19%; conversión de clic a venta: 847 / 14.592 = 5,8%.
- **Costes simulados por plataforma:** Instagram, 2.600 €; TikTok, 2.100 €; YouTube, 1.100 €. Con 9.498 € en comisiones, el ROI global es 1,64x y el coste por venta es 6,85 €.
- **Interacciones simuladas:** 28.400. Aplicando la definición de engagement global a 456.000 de alcance, la tasa de referencia es 6,2%. Un valor distinto solo es aceptable si se identifica y documenta otra base de cálculo.
- Las métricas individuales por plataforma o producto se calculan con sus propios datos atribuidos. No se debe asignar un total global a una plataforma cuando se desconoce la atribución.

## Requisitos de interfaz y tecnología

- **RT-01.** La implementación del frontend debe usar HTML y Tailwind CSS v4; se permite JavaScript vanilla únicamente para la interactividad del dashboard.
- **RT-02.** No debe incorporar React, Vue, Angular, Svelte ni otros frameworks de interfaz.
- **RT-03.** No debe usar `cdn.tailwindcss.com`, directivas `@tailwind base/components/utilities` ni configuración propia de Tailwind CSS v3. La referencia CDN permitida para el prototipo es `@tailwindcss/browser@4`.
- **RT-04.** La interfaz debe adaptarse a pantallas de escritorio y móviles sin ocultar métricas, controles o columnas esenciales; las tablas pueden desplazarse horizontalmente en pantallas estrechas.
- **RT-05.** Los controles de pestañas y listados deben poder operarse con teclado y exponer claramente el estado seleccionado.
- **RT-06.** Los estados, alertas y variaciones no deben depender únicamente del color para comunicar significado.

## Criterios de aceptación

### [x] CA-01: Estructura del dashboard

**Dado** que la usuaria abre el dashboard, **cuando** se muestra la vista principal, **entonces** encuentra exactamente tres bloques en el orden superior (KPIs), intermedio (drivers) e inferior (detalles y alertas), cada uno con un encabezado identificable.

### [x] CA-02: Modelo de comisión

**Dado** el portafolio de tres productos, **cuando** se muestra su precio y comisión unitaria, **entonces** aparecen A: 50,00 €/7,50 €, B: 120,00 €/18,00 € y C: 80,00 €/12,00 €, todos con una comisión del 15%.

### [x] CA-03: Coherencia de ventas e ingresos

**Dado** los datos de demostración, **cuando** se agregan las ventas por producto y plataforma, **entonces** ambas vistas suman 847 ventas y 9.498 € de comisiones; las ventas brutas suman 63.320 € y el ticket medio se muestra como 74,76 €.

### [x] CA-04: Tasas de rendimiento

**Dado** 14.592 clics, 456.000 impresiones, 847 ventas y 456.000 de alcance, **cuando** se calculan las tasas globales, **entonces** el CTR es 3,2%, la conversión global es 0,19% y la conversión de clic a venta es 5,8%, con sus denominadores diferenciados.

### [x] CA-05: Engagement

**Dado** 28.400 interacciones y 456.000 de alcance, **cuando** se calcula el engagement global con la definición especificada, **entonces** se muestra 6,2% (redondeado a un decimal) y no el promedio simple de tasas de plataforma.

### [x] CA-06: Diagnóstico por drivers

**Dado** datos de alcance, clics, conversiones, publicaciones e interacciones, **cuando** la usuaria consulta el bloque intermedio, **entonces** puede identificar las etapas del funnel y comparar plataformas, productos y formatos de contenido usando las métricas correspondientes.

### [x] CA-07: ROI y coste por resultado

**Dado** los ingresos y costes simulados, **cuando** se muestran eficiencia y retorno, **entonces** el ROI global es 1,64x y el coste por venta completada es 6,85 €. Si faltan costes de una entidad, su ROI figura como no disponible.

### [x] CA-08: Tablas operativas

**Dado** que la usuaria abre el bloque inferior, **cuando** selecciona Productos, Plataformas o Campañas, **entonces** se muestra la tabla correspondiente con los campos especificados y sin mezclar métricas entre pestañas.

### [ ] CA-09: Alertas y listados

**Dado** que una conversión cae de forma relevante, aparece un pico atípico o se detecta otra anomalía, **cuando** se supera el umbral de alerta configurado, **entonces** el dashboard identifica el indicador, la plataforma o campaña afectada y el período de comparación. Los listados TOP se ordenan por el criterio indicado y las oportunidades se justifican con datos.

**Estado:** Pendiente. Los umbrales están definidos y los listados TOP y las oportunidades usan datos, pero las alertas siguen siendo simuladas y no se disparan automáticamente al cruzar los umbrales.

### [x] CA-10: Responsive y tecnología permitida

**Dado** que la usuaria accede desde móvil o escritorio, **cuando** consulta las tres secciones y sus controles, **entonces** el contenido permanece legible y operable. La implementación usa HTML, Tailwind CSS v4 y JavaScript vanilla, sin frameworks de interfaz, CDN de Tailwind v3 ni directivas de esa versión.

**Estado:** Aceptado. El layout usa rejillas responsive y tablas con desplazamiento horizontal; las pestañas tienen semántica ARIA y navegación por teclado. El frontend usa HTML, Tailwind CSS v4 y JavaScript vanilla.

## Fuera de alcance

- Conexión real a APIs de Instagram, TikTok, YouTube, plataformas de afiliación o comercio electrónico.
- Autenticación, gestión de usuarios, almacenamiento persistente o edición de campañas.
- Garantizar que métricas simuladas equivalen a resultados reales de las plataformas.
