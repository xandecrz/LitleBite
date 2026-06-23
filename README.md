# LitleBite

> Landing page sencilla y responsiva para una pizzería moderna. Diseño centrado en conversión, accesibilidad y buen SEO.

## Descripción

LitleBite es una landing estática (HTML/CSS) creada para presentar un restaurante/pizzería: hero visual, menú destacado, galería, sección "Nosotros", formulario de contacto y botones para redes sociales. El objetivo es ofrecer una base limpia y optimizada para producción estática y despliegue en hosting estático (Netlify, Vercel, GitHub Pages, S3, etc.).

Este repositorio incluye estilos responsivos y prácticas básicas de SEO (meta description, canonical, sitemap.xml y robots.txt).

## Características principales

- Hero a pantalla completa con overlay y llamadas a la acción.
- Navegación con anclas: Inicio, Menu, Galería, Nosotros, Contacto.
- Sección de menú con cards responsivas.
- Galería con imágenes optimizadas.
- Sección de redes sociales con botones estilizados.
- Formulario de contacto (estático) listo para integrar con un servicio backend o formulario-service.
- SEO mínimo aplicado: meta description, canonical, sitemap.xml y robots.txt.

## Tecnologías

- HTML5
- CSS3 (variables CSS, layout responsivo con grid/flex)
- Imágenes (webp/avif)

## Estructura del proyecto

- index.html — página principal.
- css/style.css — estilos principales.
- img/ — imágenes usadas en la landing.
- sitemap.xml — sitemap para motores de búsqueda.
- robot.txt — reglas para crawlers (nota: renombrar a `robots.txt` al publicar si aplica).


## Instalación y desarrollo local

Requisitos:

- Navegador moderno.
- Servidor estático (opcional) — por ejemplo `Live Server` en VS Code o `http-server`.

Pasos:

1. Clona el repositorio:

```
git clone <tu-repo-url>
cd LitleBite
```

2. Abrir `index.html` en el navegador o ejecutar un servidor estático (recomendado):

```
# usando http-server (nodejs)
# npm i -g http-server
http-server -c-1

# o con Live Server (VS Code)
```

3. Edita `css/style.css` y las imágenes en `img/` para personalizar marca y contenidos.

## Producción / Despliegue

Esta es una aplicación estática; recomendaciones de despliegue:

- Subir a Netlify / Vercel / GitHub Pages / Amazon S3 + CloudFront.
- Asegurar que `sitemap.xml` y `robots.txt` (o `robot.txt` renombrado) queden en la raíz pública del dominio.
- Ajustar la URL `https://www.litlebite.com/` en `index.html`, `sitemap.xml` y `robot.txt` por tu dominio real.

SEO y performance (recomendaciones):

- Comprimir y servir imágenes en formatos modernos (webp/avif).
- Usar lazy-loading para imágenes de galería (`loading="lazy"`).
- Añadir etiquetas Open Graph y Twitter Card para mejorar compartido en redes.
- Habilitar caching y CDN para assets estáticos.

## SEO: sitemap y robots

- `sitemap.xml` ya incluido con rutas principales y frecuencias. Actualiza `lastmod` al publicar contenido dinámico.
- `robots.txt` permite todo el rastreo y apunta al sitemap. Cambia `Host` y `Sitemap` al publicar en el dominio final.

## Personalización rápida

- Cambiar imagen del hero: `img/hero.png` y, si es necesario, ajustar `background-position` en `css/style.css`.
- Colores: variables en `:root` en `css/style.css` (`--yellow-color`, `--black-color`, etc.).
- Reemplazar texto y enlaces del footer y botones sociales con URLs reales.

## Contribuir

1. Fork del repositorio.
2. Crear una rama con tu feature: `git checkout -b feat/nombre`.
3. Hacer commit con mensajes claros y descriptivos.
4. Abrir Pull Request explicando cambios.

## Licencia

Este proyecto no incluye licencia por defecto. Añade una licencia (MIT, Apache-2.0, etc.) si piensas compartirlo públicamente.

## Contacto

Si necesitas ayuda con personalización, despliegue o integración de un backend para el formulario de contacto, contáctame en <a href="https://xandtech.com">XandT3ch.com

---

