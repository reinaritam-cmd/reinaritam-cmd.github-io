# Blog de Simón Patiño – Guía rápida

Este proyecto es un sitio estático basado en Bulma con estilos propios centralizados y variables para facilitar personalización.

## Estructura
- `index.html`: Portada con tarjetas (cards) que contienen el contexto directamente.
- `acerca.html`: Biografía y contexto histórico.
- `images/`: Imágenes usadas en la portada y páginas.
- `css/bulma.css`: Bulma (estilos base).
- `css/blog-custom.css`: CSS generado listo para usar (variables CSS + utilidades + componentes).
- `sass/blog-custom.scss`: Fuente SASS (autoridad principal para colores y estilos).

## Estilos y variables
Los colores, tipografías, sombras y espaciados están definidos en SASS y exportados también como variables CSS.

Variables clave (definidas en `sass/blog-custom.scss` y exportadas a `:root`):
- Colores base: `--color-primary`, `--color-primary-dark`, `--color-primary-light`
- Acentos: `--color-accent`, `--color-accent-light`
- Texto: `--color-text-primary`, `--color-text-card`, `--color-text-light`, `--color-text-muted`
- Fondo y bordes: `--color-background`, `--color-white`, `--color-border`, `--color-border-light`
- Tipografía: `--font-family-serif`
- Miscelánea: `--spacing-section`, `--transition-base`, `--shadow-card`, `--shadow-card-hover`

Clases utilitarias más usadas:
- Fondo: `bg-background`, `bg-white`, `bg-light`
- Texto: `has-text-muted`
- Espaciado: `mt-2`, `mb-1`
- Hero helpers: `hero-title`, `hero-lead`
- Sección con padding: `section--padded`
- Caja de cita: `quote-box`

Componentes personalizados:
- `.hero-section`: cabecera sobria con degradado y tipografía serif
- `.card` y `.card-content`: tarjetas con sombra sutil y texto más oscuro (`--color-text-card`)

## Cómo cambiar colores/estilos
1) Edita `sass/blog-custom.scss` y modifica las variables SASS (ej. `$color-primary`, `$color-accent`).
2) Si no usas un compilador SASS: refleja los mismos cambios en `css/blog-custom.css` (misma sección `:root`).
3) Refresca el navegador.

Sugerencia: instala SASS para compilar automáticamente:
```
sass sass/blog-custom.scss css/blog-custom.css
```

## Notas
- La portada concentra el contenido; no se usan páginas de posts.
- Todo el color y estilo está centralizado en `sass/blog-custom.scss` para facilitar cambios globales.
