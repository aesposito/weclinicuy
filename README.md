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

Hay una sección "Nos eligieron" (`<section id="testimonios">`) en las dos
páginas, con **los mismos dos testimonios**: Damiana y Salomé. Si editás una
frase, cambiala en las dos páginas.

Para sumar otro: copiá el bloque `<figure class="quote-card">` entero, pegalo
justo debajo y cambiale la frase, el nombre y la foto. No hay que tocar el CSS:
las tarjetas se acomodan solas en columnas, y si queda una sola se ensancha para
no quedar flaca en el medio de la página.

En cada frase hay una parte en `<strong>`, que es la que se destaca en negrita.
Elegí un pedazo corto —media línea— y que sea el motivo por el que a alguien le
convendría alquilar acá. Si ponés media frase entera en negrita deja de
resaltar.

Las fotos van en `img/`, **cuadradas** (320×320 sirve) y encuadradas de la
cabeza a los hombros, porque se muestran chiquitas y redondas al lado del
nombre. Desde la página de odontología se escriben con `../img/` adelante.

Sólo frases reales y con permiso del profesional para usar nombre y foto.

## Galería "El lugar"

Las 4 fotos van en una fila en desktop, 2 en tablet y 1 en celular. Al hacer
click se abren grandes en un visor, con flechas y tecla Esc para salir.

Para sumar una foto: copiá un bloque `<figure class="shot">` entero. El visor
toma solas todas las que haya. En el `<button>` hay dos datos:

- `data-caption` — el texto que se lee abajo en el visor (poné el mismo que el
  `figcaption`)
- `data-full` — opcional, la versión en alta si la tenés (así está
  `recepcion.jpg` para la sala de espera). Si no la ponés, el visor agranda la
  misma foto de la grilla, así que subí las fotos de al menos 1200px de ancho.

## Equipamiento del consultorio dental

En `consultorio-odontologico-montevideo/index.html` hay un comentario marcando
dónde va la lista de equipamiento real. Está genérica a propósito. Completarla
con marcas y modelos concretos es de lo que más ayuda a posicionar esa página.
