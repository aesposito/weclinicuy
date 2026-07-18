# weclinic.uy

Sitio institucional de WeClinic — consultorios por turno en Río Branco y 18 de Julio, Montevideo.

Sitio estático, sin dependencias ni build. Se publica con GitHub Pages.

## Estructura

- `index.html` — home. Apunta a "alquiler consultorio Montevideo"
- `consultorio-odontologico-montevideo/index.html` — página de odontología.
  Apunta a "consultorio odontológico Montevideo"
- `css/site.css` — estilos compartidos por las dos páginas
- `img/` — fotos de los espacios
- `robots.txt` y `sitemap.xml` — para Google
- `CNAME` — dominio propio (weclinic.uy)

## Editar textos

Abrí el archivo desde GitHub, clic en el lápiz, cambiá el texto y guardá
("Commit changes"). En 1-2 minutos el sitio se actualiza solo.

Ojo: si cambiás el texto de una pregunta frecuente, cambiala **también** en el
bloque `application/ld+json` del `<head>` de esa misma página. Google exige que
coincidan; si no coinciden, ignora los datos estructurados.

## Si agregás una página nueva

Sumá su dirección a `sitemap.xml` y enlazala desde el menú de las otras páginas.
Una página que no está enlazada desde ningún lado casi no posiciona.

## Testimonios

Hay una sección de testimonios ya maquetada y **comentada** en `index.html`.
Está desactivada a propósito para no publicar frases inventadas. Cuando tengas
2 o 3 testimonios reales con permiso de uso, seguí las instrucciones que están
en el propio comentario.

## Equipamiento del consultorio dental

En `consultorio-odontologico-montevideo/index.html` hay un comentario marcando
dónde va la lista de equipamiento real. Está genérica a propósito. Completarla
con marcas y modelos concretos es de lo que más ayuda a posicionar esa página.
