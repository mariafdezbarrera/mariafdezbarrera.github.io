# Guía rápida: mariafdezbarrera.github.io

Esta es la plantilla Academic Pages adaptada para que la página principal tenga el mismo diseño que amughrabi.github.io.

## Publicar en GitHub
1. Crea un repositorio público llamado exactamente **mariafdezbarrera.github.io** en tu cuenta de GitHub.
2. Sube el contenido de esta carpeta (no la carpeta en sí) a la raíz del repositorio.
3. Ve a **Settings → Pages** y en "Source" elige **Deploy from a branch**, rama `master` (o `main`), carpeta `/ (root)`.
4. En 1-2 minutos estará en https://mariafdezbarrera.github.io

## Qué editar (busca "TODO")
| Qué | Dónde |
|---|---|
| Nombre, puesto, biografía, botones (Email, CV...), directores, premios, Education | `_data/home.yml` |
| Publicaciones (una por archivo) | `_publications/` |
| Charlas y pósters (una por archivo) | `_talks/` |
| Tu foto (formato vertical 4:5) | `images/profile.jpg` |
| Fotos de directores | `images/supervisor1.jpg`, `images/supervisor2.jpg` |
| Imágenes de publicaciones (16:10) | `images/pubs/` |
| CV y PDFs | `files/` (p. ej. `files/CV.pdf`) |
| Colores y tipografía | `assets/css/home.css` |

- **Publicación destacada** (`featured: true`): tarjeta con imagen y descripción.
- **Publicación normal** (`featured: false`): aparece en la lista "More publications".
- Para ocultar una sección (Awards, Research...), borra su contenido en `home.yml`. Talks/Publications se ocultan si sus carpetas están vacías.
- Para añadir secciones (Teaching, Supervision...), copia el bloque de `extra_sections` en `home.yml`.

## Ver la página en tu ordenador (opcional)
```bash
bundle install
bundle exec jekyll serve -l -H localhost
```
y abre http://localhost:4000

Las demás páginas de la plantilla original (/publications/, /talks/, /cv/...) siguen existiendo con el estilo original de Academic Pages; la portada no enlaza a ellas.
