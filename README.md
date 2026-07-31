# 🪧 El Rótulo

Landing page para un servicio de presencia en internet dirigido a negocios pequeños de Mérida, Yucatán (taquerías, estéticas, talleres, clínicas, carpinterías, salones de eventos, etc.).

Sitio de una sola página (`index.html`), sin dependencias de build ni frameworks: HTML, CSS y JavaScript vanilla. Incluye dos imágenes que deben subirse junto al `index.html`: `negocios.png` (ilustración en la sección de servicios) y `el-rotulo-og.png` (vista previa al compartir en redes).

## Contenido de la página

- **Hero** con llamada a la acción directa a WhatsApp y un mockup animado de celular que rota entre 7 ejemplos de negocios distintos.
- **Mi historia**: carrusel manual (flechas + puntos) contando el origen del proyecto en 6 pasos.
- **Servicios**: un solo bloque con tres necesidades comunes (info básica, catálogo, formulario), no paquetes cerrados.
- **Cómo funciona**: proceso en 3 pasos.
- **Beneficios**, **Transparencia de precios**, **Preguntas frecuentes** y **Contacto** con formulario que arma un mensaje de WhatsApp automáticamente.
- Botón flotante de WhatsApp en todas las vistas.

## Tecnología

- HTML5 + CSS3 (variables CSS, grid, flexbox) + JavaScript vanilla — sin librerías externas.
- Tipografías: [Fraunces](https://fonts.google.com/specimen/Fraunces) y [Work Sans](https://fonts.google.com/specimen/Work+Sans) vía Google Fonts.
- Totalmente responsive (celular, tablet, escritorio).
- Sin necesidad de servidor, build ni dependencias — es un solo archivo HTML autocontenido.

## Cómo verlo localmente

Solo abre `index.html` en cualquier navegador. No requiere instalar nada.

```bash
# Opción 1: doble clic en index.html
# Opción 2: desde terminal
open index.html        # macOS
start index.html        # Windows
xdg-open index.html     # Linux
```

## Vista previa al compartir en redes sociales

El sitio incluye una imagen de vista previa (`el-rotulo-og.png`) que aparece cuando alguien comparte el enlace en WhatsApp, Facebook, LinkedIn, Telegram o Twitter/X.

**IMPORTANTE — un paso obligatorio antes de que funcione:**

Las etiquetas de vista previa usan un placeholder `https://TU-DOMINIO.com` que **debes reemplazar** por tu URL real. Sin esto, la miniatura NO aparece (las redes sociales exigen direcciones completas, no rutas relativas).

1. Abre `index.html` y busca `TU-DOMINIO.com` (aparece **5 veces**).
2. Reemplaza las 5 por tu dirección real. Por ejemplo, si usas GitHub Pages:
   `https://tu-usuario.github.io/el-rotulo`
3. Guarda. Las 5 líneas afectadas son: `og:url`, `og:image`, `og:image:secure_url`, `twitter:image`.

Mantén el archivo `el-rotulo-og.png` en la misma carpeta que `index.html`.

**Para probar que quedó bien**, después de publicar, pega tu enlace en:
- Facebook: https://developers.facebook.com/tools/debug/
- Twitter/X: https://cards-dev.twitter.com/validator
- LinkedIn: https://www.linkedin.com/post-inspector/
- WhatsApp: simplemente envíate el enlace a ti mismo en un chat.

Si cambiaste algo y la vista previa vieja sigue apareciendo, usa el depurador de Facebook y presiona "Scrape Again" para refrescar el caché.

## Archivos del proyecto

- `index.html` — la página principal.
- `negocios.png` — ilustración de la sección de servicios.
- `el-rotulo-og.png` — imagen de vista previa al compartir en redes.
- `404.html` — página de error con la identidad de la marca (GitHub Pages la muestra sola cuando alguien entra a una URL que no existe).
- `robots.txt` — permite que Google indexe el sitio.
- `sitemap.xml` — mapa del sitio para buscadores.
- `.nojekyll` — indica a GitHub Pages que no procese el sitio con Jekyll.

Sube **todos** estos archivos juntos al repositorio, en la misma carpeta.

## Cómo publicarlo con GitHub Pages

1. Sube este repositorio a GitHub (ver pasos abajo).
2. En el repositorio, ve a **Settings → Pages**.
3. En **Source**, selecciona la rama `main` y la carpeta `/root`.
4. Guarda. En un par de minutos el sitio estará disponible en:
   `https://<tu-usuario>.github.io/<nombre-del-repositorio>/`

## Subir este proyecto a GitHub por primera vez

```bash
git init
git add .
git commit -m "Primera versión de El Rótulo"
git branch -M main
git remote add origin https://github.com/<tu-usuario>/<nombre-del-repositorio>.git
git push -u origin main
```

## Contacto del negocio

📍 Mérida, Yucatán
📱 WhatsApp: 99 91 55 82 06

---

Hecho con cariño para negocios pequeños que quieren dejar de contestar lo mismo cien veces por WhatsApp.
