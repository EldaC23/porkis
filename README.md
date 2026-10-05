# Porkis Burger · Menú digital interactivo (demo)

Un solo archivo autocontenido: `index.html` (Tailwind, FontAwesome y Google Fonts por CDN). Variante **SIN IMÁGENES**, paleta naranja `#F58220` / amarillo `#FFC21A` / base `#0E0B09`.

## Cómo funciona
- Los productos se cargan desde una hoja de Google publicada como CSV (`PRODUCTS_CSV_URL`). Si falla, usa el respaldo local `fallbackRaw` y nunca queda vacío. Avisos solo por `console.warn`.
- `menu.csv` es el contenido de la hoja (`categoria,nombre,descripcion,precio,disponible`). Importarlo en Google Sheets, `Archivo > Compartir > Publicar en la web > CSV`, y pegar la URL en `PRODUCTS_CSV_URL`.
- Para marcar un producto agotado: `disponible = no`.
- Personalización con slots en cascada (sin mostaza, sin cebolla, proteína), configurada en `CUSTOM_BY_CATEGORY` / `CUSTOM_BY_PRODUCT`.
- `WHATSAPP` y `EFECTO_LANDING_WA`: ahora son el número del demo. Cambiar `WHATSAPP` por el del negocio al entregar.
- Texto comercial: `OFERTA.md`.
