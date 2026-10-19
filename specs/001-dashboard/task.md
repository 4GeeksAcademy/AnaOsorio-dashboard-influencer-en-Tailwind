# Tareas: Dashboard de rendimiento de influencer y afiliación

## [x] Fase 1: Datos y reglas compartidas

- [x] Definir la estructura de datos para períodos, productos, plataformas, campañas, costes, ventas, clics e interacciones.
- [x] Cargar los valores de demostración descritos en `spec.md` y marcarlos como simulados.
- [x] Calcular comisión unitaria al 15% para cada producto.
- [x] Calcular ventas brutas, comisiones acumuladas y ticket medio a partir de las ventas completadas.
- [x] Calcular CTR usando clics e impresiones.
- [x] Calcular conversión global sobre alcance y conversión de clic a venta por separado.
- [x] Calcular engagement global a partir de interacciones y alcance agregados.
- [x] Calcular ROI y coste por venta; representar costes ausentes como no disponibles.
- [x] Aplicar período seleccionado y formatos de números/moneda a todas las métricas.
- [x] Comprobar que los totales simulados por producto y plataforma coinciden.

## [x] Fase 2: Bloque superior — KPIs principales

- [x] Crear el encabezado del bloque de visión ejecutiva.
- [x] Mostrar ventas completadas, inscripciones, usuarios activos e impresiones.
- [x] Mostrar comisiones acumuladas, ventas brutas y ticket medio.
- [x] Mostrar engagement, interacciones, CTR y conversión global.
- [x] Mostrar ROI y coste por venta completada con sus unidades.
- [x] Añadir comparación con el período anterior cuando haya datos disponibles.
- [x] Indicar de forma comprensible si cada variación es positiva, negativa o neutra.

## [x] Fase 3: Bloque intermedio — Drivers del resultado

- [x] Crear el funnel con alcance, clics y ventas completadas.
- [x] Mostrar las tasas alcance-clics y clics-ventas junto con los volúmenes.
- [x] Comparar alcance, conversiones e ingresos por plataforma.
- [x] Comparar ventas, comisiones y tasa de conversión para A, B y C.
- [x] Mostrar volumen de publicaciones e interacciones por formato de contenido.
- [x] Usar totales agregados al calcular tasas globales, sin promediar porcentajes de plataformas.
- [x] Señalar datos de atribución desconocida sin asignarlos arbitrariamente a una plataforma o campaña.

## [x] Fase 4: Bloque inferior — Detalle operativo y alertas

- [x] Crear la tabla de productos con precio, comisión unitaria, conversiones, comisiones y ROI.
- [x] Crear la tabla de plataformas con alcance, engagement, conversiones y plataforma TOP.
- [x] Crear la tabla de campañas con fechas, producto, resultados y rendimiento.
- [x] Permitir consultar las tres tablas por separado mediante controles operables.
- [x] Definir umbrales para caída de conversión, picos atípicos y anomalías.
- [x] Mostrar en cada alerta el indicador, la entidad afectada y el período de comparación.
- [x] Crear el listado TOP Productos ordenable por su métrica de referencia.
- [x] Crear el listado TOP Plataformas ordenable por su métrica de referencia.
- [x] Crear el listado TOP Campañas ordenable por su métrica de referencia.
- [x] Mostrar oportunidades de mejora justificadas por los datos observados.

## [x] Fase 5: Revisión transversal y aceptación

- [x] Mantener los tres bloques en el orden definido por `spec.md`.
- [x] Adaptar tarjetas, controles y tablas a pantallas móviles y de escritorio.
- [x] Habilitar el uso por teclado y exponer el estado seleccionado de los controles.
- [x] Comunicar estados y alertas sin depender únicamente del color.
- [x] Verificar los criterios CA-01 a CA-10 de `spec.md` con los datos de demostración.
- [x] Confirmar que la interfaz usa HTML, Tailwind CSS v4 y JavaScript vanilla, sin frameworks ni configuración de Tailwind v3.
