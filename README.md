# 📊 Dashboard de Rendimiento — Influencer & Afiliación

> **Instrucción para Copilot:** utiliza únicamente HTML y Tailwind CSS v4. No añadas React, Vue ni otros frameworks, no uses `cdn.tailwindcss.com` y no incluyas directivas ni configuración de Tailwind CSS v3.

Dashboard interactivo para seguimiento de métricas de redes sociales y ventas de afiliación, diseñado para una influencer con presencia en múltiples plataformas (Instagram, TikTok, YouTube).

## 🚀 Tecnologías

- **HTML5** — Estructura semántica
- **Tailwind CSS v4** — Utilidades cargadas mediante `@tailwindcss/browser@4`
- **JavaScript vanilla** — Interactividad ligera integrada en el HTML
- **Flask (Python)** — Servidor de desarrollo

> No se usan frameworks como React, Vue, Angular o Svelte. El proyecto no utiliza el CDN `cdn.tailwindcss.com` ni configuración de Tailwind v3.

## 📋 Contenido

| Archivo | Descripción |
|---|---|
| `index.html` | Dashboard principal con 3 bloques visuales (KPIs, Drivers, Detalles) |
| `PROPUESTA.md` | Propuesta formal del proyecto |
| `server.py` | Servidor Flask para desarrollo |

## 🏗️ Estructura del Dashboard

### Bloque Superior — KPIs Principales (Visión Ejecutiva)
- Volumen (ventas, inscripciones, usuarios activos, impresiones)
- Ingresos (revenue/comisiones, ticket medio)
- Engagement & Rendimiento (tasa engagement, CTR, conversión)
- Eficiencia & Retorno (ROI, coste por resultado)

### Bloque Intermedio — Drivers del Resultado (Diagnóstico)
- Funnel de Conversión (Alcance → Clics → Ventas)
- Rendimiento por Plataforma (Instagram vs TikTok vs YouTube)
- Rendimiento por Producto (Productos A, B, C)
- Actividad vs. Engagement (publicaciones vs interacciones)

### Bloque Inferior — Detalles Operativos (Acción)
- Tablas detalle (Productos, Plataformas, Campañas)
- Sistema de Alertas Automáticas
- Listados TOP (Productos, Plataformas, Campañas, Oportunidades)

## 🚀 Cómo ejecutar

```bash
pip3 install flask && python3 server.py
```

Luego abre `http://localhost:3000` en tu navegador.

## 🎯 Modelo de Negocio

- Comisión fija del **15%** por venta completada
- **Producto A:** 50 € → 7,50 € comisión
- **Producto B:** 120 € → 18,00 € comisión
- **Producto C:** 80 € → 12,00 € comisión

---

*Dashboard desarrollado con ❤️ · HTML + Tailwind CSS v4 + JavaScript vanilla*
