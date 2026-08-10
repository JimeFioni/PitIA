# pitia-web

Sitio de **PitIA** — Ingeniería de negocios e IA.
Córdoba, Argentina. → https://pitia.com.ar

## Estructura

```
index.html            Sitio completo: HTML, CSS y JS en un solo archivo
og.png                Imagen que se muestra al compartir el link
assets/fotos/         Fotos de las socias
```

Sin dependencias, sin compilación, sin `npm install`. Se abre el
archivo en el navegador y funciona.

## Cómo modificar el contenido

Todo el texto está en `index.html`. Las secciones están marcadas con
comentarios (`<!-- ══ HERO ══ -->`, `<!-- ══ MÉTODO ══ -->`, etc.).

Para cambios de texto se puede editar directamente desde GitHub:
abrir el archivo → ícono del lápiz → editar → *Commit changes*.
Netlify publica el cambio solo, en menos de un minuto.

## Colores y tipografías

Están todos declarados una sola vez, al principio del `<style>`, en
`:root`. Cambiar un color ahí lo cambia en todo el sitio.

```
--ink       #1B2A33   texto principal, fondos oscuros
--accent    #56684E   laurel: acento, la respuesta
--paper     #F4F2EC   fondo principal
--deep      #16221B   fondo de secciones oscuras
```

Tipografías: Spectral (títulos), Public Sans (texto), IBM Plex Mono
(etiquetas y numeración). Se cargan desde Google Fonts.

## Pendientes antes de publicar

Buscar y reemplazar en `index.html`:

- [ ] `TU_ID_DE_FORMSPREE` → id real del formulario (formspree.io)
- [x] Teléfonos cargados: Jime +54 9 353 240-2451 · Xime +54 9 353 402-5886
- [ ] `54XXXXXXXXXX` → número del botón de WhatsApp
- [ ] `https://VIALPARKING-URL` → sitio de VialParking
- [ ] Plazos de las cuatro etapas del método (sección Cómo trabajamos)

## Publicación

Netlify conectado a este repositorio. Cada push a `main` publica.
Dominio `pitia.com.ar` delegado desde NIC.ar a los servidores de
nombres que indica Netlify. Certificado SSL automático.

## Reglas de marca que afectan al código

- El nombre se escribe siempre `Pit<b>IA</b>`, con la I y la A destacadas.
- El punto del isotipo nunca va arriba de la bóveda.
- El laurel (`--accent`) se reserva para acentos, no como fondo de bloque.
- Toda animación debe respetar `prefers-reduced-motion`.
