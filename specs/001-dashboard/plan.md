# Plan de implementación: Dashboard de rendimiento

## Objetivo

Implementar el dashboard definido en `specs/001-dashboard/spec.md`, respetando sus tres bloques visuales, reglas de negocio y criterios de aceptación. La interfaz se construirá con HTML, Tailwind CSS v4 y JavaScript vanilla, sin frameworks de UI ni configuración de Tailwind CSS v3.

## Orden de implementación

### 0. Datos y reglas compartidas

Establecer una estructura común para período, productos, plataformas, campañas, costes, ventas, clics e interacciones. Cargar los valores de demostración identificándolos como simulados y usar funciones compartidas para calcular:

- Comisión unitaria: precio × 15%.
- Ventas brutas y comisiones acumuladas a partir de ventas completadas.
- Ticket medio: ventas brutas / ventas completadas.
- CTR: clics / impresiones.
- Conversión global: ventas / alcance; conversión de clic a venta: ventas / clics.
- Engagement global: interacciones agregadas / alcance agregado.
- ROI: comisiones / costes atribuibles.
- Coste por resultado: costes atribuibles / ventas completadas.

Los datos agregados deben coincidir por producto y plataforma. Si faltan costes, el ROI debe mostrarse como no disponible. El período seleccionado y el formato local de euros se aplicarán de manera uniforme.

### 1. Bloque superior: KPIs principales

Construir la visión ejecutiva con métricas de volumen, ingresos, engagement y rendimiento, eficiencia y retorno. Mostrar ventas brutas junto a comisiones, y explicar la unidad del coste por resultado. Añadir comparación con el período anterior cuando los datos estén disponibles, indicando la dirección de la variación con texto y no solo con color.

### 2. Bloque intermedio: drivers del resultado

Implementar el funnel alcance → clics → ventas con volúmenes y tasas. Añadir comparativas de plataformas por alcance, conversiones e ingresos; de productos por ventas, comisiones y conversión; y de actividad por formato frente a interacciones. Calcular porcentajes globales con totales agregados y no asignar ventas a una plataforma o campaña cuando su atribución sea desconocida.

### 3. Bloque inferior: detalle operativo y alertas

Implementar las tablas de productos, plataformas y campañas según los campos de la especificación, con controles que permitan consultar cada vista por separado. Añadir los listados TOP ordenables por una métrica explícita y oportunidades de mejora justificadas con datos. Configurar alertas de caída de conversión, picos atípicos y otras anomalías; cada alerta debe identificar métrica, entidad afectada y período comparado.

### 4. Revisión transversal

Comprobar que los tres bloques se presentan en el orden especificado y que el dashboard funciona en móvil y escritorio. Verificar operación por teclado, estado seleccionado de los controles y comunicación de estados sin depender únicamente del color. Confirmar el cumplimiento de los criterios CA-01 a CA-10.

## Decisión pendiente

La especificación requiere umbrales configurables para las alertas, pero no fija valores numéricos. Acordar esos umbrales antes de validar las alertas contra datos reales.

## Fuera de alcance

La implementación descrita no incluye conexión con APIs reales, autenticación, persistencia ni gestión de usuarios. Los datos del prototipo deben seguir identificándose como simulados hasta disponer de fuentes conectadas.
