# Adaptogenesis — Rediseño Web E-commerce

Rediseño de **Adaptogenesis / The Adaptogenic Lifestyle**, actualmente en Wix, migrando de un sitio denso a una **botica artesanal y clínica botánica de lujo orgánico** (estilo *Aesop* o *Flamingo Estate*).

- **Sitio actual:** https://www.adaptogeniclifestyle.com/ (Wix)
- **Fundadora:** Abbie Jean Ciullo — CFNC, MCS-P
- **Dirección estética aprobada:** botica de lujo orgánico y medicina de terreno. Nada de estética SaaS o software.
- **Enfoque:** diseño responsive (desktop editorial + mobile), padding lateral amplio, tipografía serif editorial y fondos de lino cálido/pergamino.

Este repo contiene 3 prototipos HTML navegables (generados con Google Stitch, versión responsive) que materializan esa dirección, listos para desplegarse como sitio estático en Vercel.

## Páginas

| Archivo | Pantalla | Descripción |
|---|---|---|
| [`index.html`](./index.html) | **Home** | Landing editorial de escritorio con header sticky, hero split 55/45, grid asimétrico de productos y bio de Abbie Jean Ciullo. |
| [`collection.html`](./collection.html) | **Dispensary Archive** (Collection Template) | Header con drawer mobile, fórmula insignia (*Signature Reserve*) y grid multi-columna de remedios. |
| [`product.html`](./product.html) | **Rise Elixir** (PDP Template) | Layout de dos columnas con galería + panel de compra sticky, compra única vs. suscripción (*Cyclical Dispatch*), activos botánicos y sinergias clínicas. |

Las tres pantallas están enlazadas entre sí (logo, nav "Dispensary" y tarjetas de producto) para poder navegar el prototipo como un sitio real. Cada plantilla es responsive: se adapta desde mobile hasta escritorio ancho (`max-w-7xl` / `container-max`), a diferencia de la primera entrega (mobile-only).

Capturas de referencia de cada pantalla en [`previews/`](./previews).

## Sistema de diseño — "Botanical Vitality"

Documentado en [`DESIGN.md`](./DESIGN.md) (tokens de color, tipografía, espaciado, sombras, componentes).

- **Paleta:** pergamino/lino cálido (`#FBF9F5`, `#FEF9F0`), verde oliva bosque (`#32533C` / `#4A6B53`), tinta carbón (`#1B2A22`), acentos en terracota (`#C86D51`) y ámbar botánico.
- **Tipografía:** `EB Garamond` / `Cormorant Garamond` para encabezados editoriales (cursivas para conceptos clave), `Plus Jakarta Sans` para cuerpo y UI.
- **Espaciado y forma:** grids holgados (`px-5` / `px-6`), esquinas suaves (4–8px), bordes de 1px en tono lino, cero sombras marcadas.

## Estructura y contenido de cada pantalla

### A. Homepage (Boutique & Clínica)
- **Hero:** frasco ámbar sobre piedra y plantas secas. *"Cellular resilience cultivated through whole-organism gut metagenomics and sun-cured desert adaptogens."*
- **Síntomas en grid sintético:** chips de 2 columnas (*Digestive bloat*, *Chronic fatigue*, *Hormone shifts*, *Brain fog*).
- **The Dispensary:** *Rise Elixir* ($48), *Digestive Bitters* ($34), *Cardon Essence* ($28) y kit clínico *BiomeFx* ($395).
- **Historia de Abbie:** autoridad clínica (CFNC, MCS-P) y los 4 pilares — *Terrain Inquiry*, *BiomeFx Analysis*, *Botanical Blending*, *1:1 Integration*.
- **Captura de leads:** guía de 6 pasos para la salud digestiva.

### B. Collection Page (The Dispensary Archive)
- **Header:** manifiesto de cosecha en Baja California Sur y preservación en vidrio violeta Miron.
- **Filtros:** *All Formulations*, *Dual-Extracts*, *Daily Remedies & Tonics*.
- **Card destacada (Signature Reserve):** ficha prioritaria para *Rise Elixir* con potencia de extracción (1:2 whole plant).
- **Grid de productos:** tarjetas con lote, volumen y botón discreto `+ Bag`.
- **Ficha clínica especial:** kit *BiomeFx™ Metagenomic Gut Profile* con secuenciación y videoconsulta de 60 min.

### C. PDP (Rise Elixir)
- **Galería visual:** botella ámbar, gotero botánico y notas de laboratorio.
- **Selector de compra:** *Cyclical Dispensary Dispatch* (suscripción, 15% OFF — $40.80) vs. *Single Bottle Purchase* ($48.00).
- **"The Terrain Purpose":** mecanismo del eje HPA y vitalidad mitocondrial sin cafeína.
- **Acordeones clínicos:** *Botanical Actives & Provenance*, *The Daily Ritual & Application*, *Extraction Methodology*.
- **Cross-sell:** *Pairs in Clinical Practice* (Digestive Bitters y Cardon Essence).
- **Terrain Notes:** reseñas de clientes verificados.

## Stack

Prototipos estáticos HTML + [Tailwind CSS (CDN)](https://cdn.tailwindcss.com) + Google Fonts (`EB Garamond`, `Plus Jakarta Sans`) + Material Symbols. Sin build step — se despliegan directamente como sitio estático.

## Deploy

```bash
vercel --prod
```

---

🤖 Repositorio y despliegue generados con [Claude Code](https://claude.com/claude-code)
