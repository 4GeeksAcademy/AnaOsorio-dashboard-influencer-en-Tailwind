# 📊 Propuesta de Dashboard de Rendimiento — Influencer & Afiliación

**Cliente:** Influencer · Redes Sociales & E-commerce  
**Formato:** HTML + Tailwind CSS v4  
**Período de análisis:** Octubre 2026

> **Instrucción para Copilot:** trabajar únicamente con HTML y Tailwind CSS v4. No incorporar React, Vue ni otros frameworks; no usar `cdn.tailwindcss.com` ni instrucciones de Tailwind v3.

---

## 1. Resumen Ejecutivo

Se propone un **Dashboard Visual e Interactivo** que unifica la información fragmentada entre plataformas sociales (Instagram, TikTok, YouTube) y los datos de ventas por afiliación. El tablero está diseñado para que **tomes decisiones rápidas** sin necesidad de abrir 5 herramientas distintas.

> 🎯 **Objetivo:** Centralizar métricas de *alcance, engagement, conversión e ingresos* en una sola vista, permitiendo identificar qué productos, plataformas y campañas rinden mejor.

---

## 2. Modelo de Negocio — Tu Máquina de Ingresos

| Concepto | Detalle |
|---|---|
| **Modelo** | Promoción de productos mediante links/códigos de afiliación en redes sociales |
| **Comisión** | **15% fija** por cada venta completada |
| **Ticket medio simulado** | 74,76 € |
| **Ventas brutas simuladas** | 63.320 € |
| **Comisiones simuladas** | 9.498 € |

### Portafolio de Productos

| Producto | Precio | Comisión Unitaria (15%) | Margen |
|---|---|---|---|
| **Producto A** | 50,00 € | 7,50 € | 15% |
| **Producto B** | 120,00 € | 18,00 € | 15% |
| **Producto C** | 80,00 € | 12,00 € | 15% |

> 💡 **Dato clave:** El Producto B genera más del doble de comisión por venta que el Producto A. ¿Dónde enfocar tu contenido?

---

## 3. Estructura del Dashboard — 3 Bloques Estratégicos

### 📊 BLOQUE SUPERIOR — KPIs Principales (Visión Ejecutiva)

Métricas de un vistazo para saber *cómo va el negocio* sin perder tiempo.

| Categoría | Métricas |
|---|---|
| **Volumen** | Ventas totales, inscripciones, usuarios activos, impresiones |
| **Ingresos** | Revenue (comisiones acumuladas), ventas totales, ticket medio de venta |
| **Engagement & Rendimiento** | Tasa de engagement global, interacciones totales, CTR, tasa de conversión |
| **Eficiencia & Retorno** | Retorno por plataforma (ingresos / costes), coste por resultado |

### 📊 BLOQUE INTERMEDIO — Drivers del Resultado (Diagnóstico)

Para entender *por qué* pasan las cosas y qué palancas mover.

| Sección | Qué muestra |
|---|---|
| **Funnel de Conversión** | Alcance → Clics → Ventas (tasas de paso entre etapas) |
| **Rendimiento por Plataforma** | Comparativa Instagram vs TikTok vs YouTube vs Otras |
| **Rendimiento por Producto** | Comisiones y conversión de los 3 productos lado a lado |
| **Actividad vs. Engagement** | Publicaciones vs Interacciones — ¿está rindiendo tu esfuerzo? |

### 📊 BLOQUE INFERIOR — Detalles Operativos y Alertas (Acción)

Para tomar decisiones concretas y no perder detalle.

| Sección | Qué incluye |
|---|---|
| **Tablas de Detalle** | Productos (precio, comisión, conversiones, ROI) · Plataformas (alcance, engagement) · Campañas (fechas, producto, resultados) |
| **Alertas Automáticas** | Caídas bruscas en conversión, picos atípicos, anomalías de rendimiento |
| **Listados Rápidos** | TOP Productos · TOP Plataformas · TOP Campañas · Oportunidades de Mejora |

---

## 4. Stack Tecnológico

| Tecnología | Versión / Uso |
|---|---|
| **HTML5** | Estructura semántica del dashboard |
| **Tailwind CSS v4** | Framework CSS utility-first via CDN (`@tailwindcss/browser@4`) |
| **JavaScript vanilla** | Interactividad ligera integrada en el HTML (sin frameworks) |
| **Flask (Python)** | Servidor de desarrollo local |

> 🚫 **Excluido explícitamente:** React, Vue, Angular, Svelte y cualquier framework de UI. No se debe usar `cdn.tailwindcss.com` ni directivas/configuración de Tailwind v3.

---

## 5. Próximos Pasos (Roadmap)

| Fase | Acción |
|---|---|
| **Fase 1** | Diseño visual del dashboard con datos simulados (este documento) |
| **Fase 2** | Conexión a fuentes reales (API de Instagram, TikTok, YouTube, Google Analytics) |
| **Fase 3** | Automatización de alertas y reportes programados |
| **Fase 4** | Panel de control interactivo con filtros en tiempo real |

---

## 6. Beneficios Esperados

- ⏱ **Ahorro de tiempo:** De 5 herramientas a 1 sola vista
- 📈 **Identificación rápida** de qué producto/platforma/campaña funciona mejor
- 🚨 **Alertas tempranas** para corregir caídas de rendimiento
- 💰 **Maximización de ingresos** al enfocar esfuerzos donde más renta

---

📊 *Propuesta preparada por Consultoría de Business Intelligence · Octubre 2026*