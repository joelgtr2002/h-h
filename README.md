# Sitio web de H&H Construcciones

Sitio estático, responsive y preparado para GitHub Pages.

## Abrir en Visual Studio Code

1. Descomprima la carpeta.
2. Abra `hh-invernaderos-web` en Visual Studio Code.
3. Instale opcionalmente la extensión **Live Server**.
4. Abra `index.html` directamente o use **Open with Live Server**.

## Cambiar WhatsApp y correo

En `index.html`, busque `EDITE el número`. Reemplace:

- `https://wa.me/593XXXXXXXXX` por el número completo, sin `+`, espacios ni guiones.
- `+593 XXX XXX XXX` por el texto que se verá.
- `correo@ejemplo.com` en el enlace y en el texto visible.

Ejemplo de WhatsApp: `https://wa.me/593991234567`.

## Agregar fotografías a “Nuestros trabajos”

1. Cree la carpeta `assets/img/trabajos/`.
2. Copie allí imágenes WebP o JPG optimizadas (ideal: 1200–1600 px de ancho y menos de 300 KB).
3. En `index.html`, localice `GALERÍA EDITABLE`.
4. Reemplace un botón provisional por este formato:

```html
<button class="project-card__media" type="button"
        data-full="assets/img/trabajos/invernadero-01.webp"
        aria-label="Abrir imagen del invernadero de Latacunga">
  <img src="assets/img/trabajos/invernadero-01.webp"
       width="1200" height="800" loading="lazy"
       alt="Invernadero construido en Latacunga">
</button>
```

Cambie también el título, categoría y ubicación. Para agregar otra obra, duplique un bloque completo `<article class="project-card">...</article>`.

## Publicar gratis en GitHub Pages

1. Cree un repositorio público en GitHub.
2. Suba el contenido de esta carpeta a la raíz del repositorio.
3. Abra **Settings → Pages**.
4. En **Build and deployment**, elija **Deploy from a branch**.
5. Seleccione la rama `main` y la carpeta `/ (root)`.
6. GitHub mostrará la URL cuando termine la publicación.

## Personalización rápida

Los colores están al inicio de `styles.css`, dentro de `:root`. El diseño usa HTML5, CSS moderno y JavaScript nativo, sin dependencias externas.
