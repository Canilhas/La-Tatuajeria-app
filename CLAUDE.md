# La Tatuajeria · Artink Tattoo — app web

App móvil (PWA) para **La Tatuajeria / Artink Tattoo**, estudio de tatuajes y piercings en **Moncada (Valencia)**. Cliente de Pedro Canilhas (Canilhas Visuals). Instagram del estudio: `@la_tatuajeria_artinktattoo`.

- Publicada en GitHub Pages: https://canilhas.github.io/La-Tatuajeria-app/
- Rama `main` = producción. Cada push a `main` se publica solo en 1–2 minutos.
- Idioma de la app y de las conversaciones con Pedro: **español**.

## Estructura

Todo vive en un único archivo autocontenido, sin build ni dependencias:

- `index.html` — HTML + CSS + JS de toda la app. Las imágenes (fotos del estudio) van incrustadas en base64, por eso el archivo pesa ~570 KB. No reescribas el archivo entero: edita por partes.
- `manifest.json` + `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — instalación en pantalla de inicio.
- `.nojekyll` — necesario para GitHub Pages; no borrar.

Pantallas (secciones `id="s-..."`, navegación con barra inferior Inicio · Presupuesto · Info):

- `s-inicio` — hero, tarjetas Tatuajes / Piercings (llevan al presupuesto con el tipo preseleccionado), horario, galería "Conoce La Tatuajeria" con lightbox.
- `s-presupuesto` — formulario tatuaje/piercing → genera resumen y enlace de WhatsApp (`#wa-link`).
- `s-info` — pestañas FAQ (`i-faq`), Mapa del dolor (`i-dolor`), Proceso y cuidados (`i-proceso`).

## Configuración clave (en `index.html`)

- **WhatsApp del estudio:** `https://wa.me/34677444696` (se rellena con el mensaje del presupuesto).
- **Horario:** L–V 10:00–14:00 · 16:00–20:00, sábado 10:00–14:00, domingo cerrado. Solo con cita previa.

## Estilo visual

- Colores (variables CSS): `--ink #14100D`, `--paper #EFE6D4`, `--red #C03A2B`, `--red-deep #8E2A1F`, `--gold #F7DC07`, `--smoke #9A8F7F`. Fondo/tema `#0D0A08`.
- Tipografías (Google Fonts): Alfa Slab One, Allura, Yellowtail, Work Sans.
- Estética de estudio de tatuaje tradicional/old school. Mantener esa línea en cualquier cambio.

## Forma de trabajar

- Antes de publicar, comprobar el cambio en vista móvil y enviar a Pedro la preview del `index.html` para que lo revise.
- Commits pequeños y descriptivos en español.

## Historial

- Nov 2026: eliminada la pestaña "Servicios" (grid de trabajos / feed de Instagram) a petición de Pedro.

## Pendientes conocidos

- Revisar si las fotos de la galería del estudio son definitivas.
