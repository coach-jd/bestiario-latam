# El Bestiario del Emprendimiento Latinoamericano — Libro Web™

Este proyecto es un **Libro Web**: un sitio estático que se lee por
capítulos, se instala como app y funciona sin conexión. Esta guía es para
quien lo mantiene; no hace falta saber programar para lo habitual.

## Estado de este proyecto

- **Imágenes pendientes:** 28 (11 heros y 17 de apoyo) — ver `prompts-imagenes.md`. Portada y foto del autor ya están.
- **Leads:** configurados con el servicio PHP del dominio (`libro_web/correo/enviar.php?libro=bestiario-latam`). Falta el renglón en `config.php` del servidor.
- **Por revisar del autor:** subtítulos agregados, correcciones del «sino», diagnóstico completo, bio del autor y textos del correo (`email/plantilla-diagnostico.html`).

## Qué hay en la carpeta

```
index.html              la página (casi nunca se edita)
ver-libro.bat           abre el libro en tu computadora (Windows, doble clic)
data/content.json       TODO el contenido: título, capítulos, textos, diagnóstico
css/styles.css          colores y tipografía (bloque :root, al principio)
css/custom.css          estilos propios de este libro (no los pisa ninguna actualización)
images/                 las imágenes del libro
prompts-imagenes.md     una ficha por imagen, con su prompt listo para copiar
email/                  plantilla del correo de resultado (si hay diagnóstico)
icons/                  íconos de la app instalable
js/app.js               el motor (no se edita)
manifest.json           nombre e íconos de la app instalable
service-worker.js       lectura sin conexión
```

## Verlo en tu computadora

El libro no funciona bien abriendo `index.html` con doble clic: necesita un
servidor local encendido. Si ves recuadros punteados donde ya guardaste una
imagen, casi siempre es porque ese servidor no está corriendo.

- **En Windows:** haz doble clic en `ver-libro.bat` y deja abierta la
  ventana que aparece.
- **En cualquier sistema:** abre una terminal en esta carpeta y ejecuta:

```bash
python -m http.server 8080
```

Después abre `http://localhost:8080` en el navegador. (En Mac o Linux el
comando es `python3`.)

## Agregar las imágenes

1. Abre `prompts-imagenes.md`. Cada imagen pendiente tiene un bloque de
   código con su prompt.
2. Copia ese bloque completo (desde `{` hasta `}`) y pégalo en tu generador
   de imágenes.
3. Guarda el resultado en `images/` con **exactamente** el nombre del título
   de su ficha (por ejemplo `images/capitulo-1-hero.jpg`).
4. Cambia su **Estado** de `pendiente` a `lista` en el documento.
5. Recarga el libro: la imagen reemplaza sola al recuadro punteado.

Usa JPG, de unos 1600 px de ancho y menos de 400 KB por imagen.

## Editar el texto

Todo el contenido está en `data/content.json`. Ábrelo con un editor de
texto y cambia lo que está entre comillas. Cuida de no borrar comillas,
comas ni llaves: es un formato estricto. Si algo deja de verse, deshaz el
último cambio.

- `**texto**` resalta en el color de acento.
- `[texto](https://ejemplo.com)` crea un enlace.
- No cambies los `"id"` de los capítulos de un libro ya publicado: los
  lectores perderían su progreso.

## Recibir los datos de los lectores

Los formularios (correo y diagnóstico) envían los datos al destino que
indica `"leads"` dentro de `"meta"` en `data/content.json`. Si ese bloque
no existe, el libro está en **modo demo** y los datos no llegan a nadie.

Lo estándar es el servicio de correo PHP del dominio (carpeta
`libro_web/correo/` del servidor), que envía por SMTP y guarda cada lead en
un CSV. En `meta.leads.webhook` va la dirección de su `enviar.php` y en su
`config.php` (en el servidor) el renglón de este libro. La carpeta `email/`
de este proyecto se sube con el libro: de ahí sale el diseño del correo.

Alternativa sin PHP, con EmailJS:

1. Crea una plantilla en EmailJS y pega el contenido de
   `email/plantilla-diagnostico.html`.
2. En la plantilla: *To Email* `{{to_email}}`, tu correo en *Reply To* y en
   *Bcc*, y el asunto que prefieras.
3. Copia a `data/content.json` → `meta.leads.emailjs` tu Service ID, tu
   clave **pública** y el Template ID. Nunca pongas la clave privada.
4. En `meta.url` escribe la dirección final del libro: de ahí salen las
   imágenes del correo. Los correos de prueba enviados desde tu computadora
   llegan sin imágenes; es normal.
5. En EmailJS, limita los envíos al dominio de tu libro.

## Publicarlo

Es un sitio estático: sube la carpeta completa a cualquier hosting.

- **Netlify Drop** (app.netlify.com/drop): arrastra la carpeta y obtienes
  un enlace en segundos. Después puedes conectar tu dominio.
- **Vercel** o **GitHub Pages**: alternativas equivalentes.

Una vez publicado con `https://`, los lectores pueden instalarlo con el
botón **"Descargar la app"** que está al final del índice.

**Para que al compartir el enlace se vea la portada:** escribe la dirección
final en `data/content.json` → `meta.url` (por ejemplo
`"url": "https://libro.midominio.com/"`) y pide que se vuelva a ejecutar la
configuración del proyecto (`setup_book.py`) antes de subirlo. La imagen que
se muestra es `images/compartir.jpg`.

## Publicar una actualización

Los cambios de texto e imágenes se ven en la siguiente visita de cada
lector. Si cambiaste colores o el diseño (`css/` o `js/`), sube además el
número de versión en `service-worker.js` (`CACHE_NAME`, por ejemplo de
`-v1` a `-v2`) para que todos reciban la versión nueva.
