# ¿Como puedo contribuir?

De momento la mejor manera de ayudar es traduciendo una sección de *switching.social*.

## Como traducir

1. Haz un *fork* de este proyecto en GitHub.
2. Dirígete a la carpeta `versiones archivadas`.
3. Escoje una pagina a traducir, puedes escojer dentro de la crpeta `convertidos a md` ó `switching.software-master por rosnovsky`.
4. Si escojiste una pagina que esta en html, conviértela a markdown (explicación de como hacer esto más adelante). Usa la terminación `.md` para consistencia dentro del proyecto. Asegúrate que el archivo tiene un nombre descriptivo, más detalles abajo.
5. Traduce el texto al inglés. Mantén solo el contenido, borra el encabezado y la información adicional del sitio (Ejemplo: borra el encabezado que contiene"Skip to content", "Ethical alternatives to popular sites and apps", "About this Site". Tmabien borra el contenido del final como "back to the front page" y " about this site / F.A.Q. / CC BY-SA 4.0 by switching.social") Un ejemplo de que borrar y que mantener se encuentra abajo.
6. Cuando termines de traducir mueve el archivo al directorio `textos traducidos`. Recuerda que esta carpeta esta un nivel arriba que `versiones archivadas`.
7. La traducción esta lista! Ahora solo falta mandar un *pull request* para agregar tus cambios al repositorio principal.

### ¿Como transformar una pagina de HTML a Markdown?

1. Asegúrate que tu *fork* este en tu disco duro, guardado locamente.
2. Baja la herramienta *pandoc*.

> [Descarga *pandoc*](https://github.com/jgm/pandoc/releases/latest) para PC, Mac y Windows desde GitHub.
> 
> Lee la [documentación](https://pandoc.org/MANUAL.pdf) de *pandoc*.

3. Usa pandoc para transformar `index.html` a `done.md`, usa el siguente comando, solo copia y pega en la linea de comando dentro del directorio del archivo que buscas convertir:

```
pandoc.exe .\index.html -f html -t markdown -o done.md
```

> Esto generará un nuevo archivo llamado `done.md`, basate en este archivo para traducir.

4. Una vez la traducción este completa re-nombra el archivo a un nombre apropiado, ejemplo:

> Antes: `about-this-site\index.html`, después: `about-this-site\about-this-site.md`.

5. Continua las instrucciones de traducción, reanuda en el paso numero *5*.


### ¿Que elementos eliminar y que elementos conservar de una traducción?

Conserva:

* Contenido
* Texto explicativo
* Imágenes, videos y media embebida con el propósito de aclarar la tesis del texto
* Hiper-vínculos ó ligas

Elimina:

* El *header*: Todos los elementos de la parte superior (logotipo, linea de división de logo/contenido, liga a la pagina principal).
* El *footer*: Todos los elementos después de, abajo de, el contenido (la liga a la pagina principal, la linea de división inferior, la sección de ligas; acerca del sitio, preguntas frecuentes, licencia y autor original).

Un ejemplo visual:

> Antes de eliminar el *header* y *footer*.

![foto](/imágenes/con-header.JPG)

> Después de eliminar el *header* y *footer*.

![foto](/imágenes/sin-header.JPG)

> Después de transformar a Markdown.


```
# Ethical alternatives to Instagram

## PixelFed

An [open source][1] [federated][2] alternative to Instagram, PixelFed is a photo-oriented social network with filters, comments, likes, shares etc. but no ads and no tracking. You can see an [example of a PixelFed account here][3], and an [example post here][4].

[1]: https://switching.software/what-is-open-source-software/
[2]: https://switching.software/federated-sites/
[3]: https://pixelfed.social/earth
[4]: https://pixelfed.social/p/earth/22346

The network is made up of lots of independent sites that talk to each other, so you can sign up on any PixelFed site and follow people on the network’s other sites too. (It doesn’t matter if you join a big or small site, they’re all part of the same network.)

Also, because PixelFed sites connect together using the ActivityPub standard, you can follow millions of people on other ActivityPub sites like [Mastodon][5], and they can follow you too.

[5]: https://switching.software/ethical-alternatives-to-facebook/

Unlike Instagram, you don’t need an app to use PixelFed, it works through your browser on phones, computers and tablets. (There are also apps in development for people who prefer them.)

**WHERE TO SIGN UP** – [pixelfed.de][6], [pix.tedomum.net][7], [pix.diaspodon.fr][8] and many others

**EXAMPLE ACCOUNT** – [@earth@pixelfed.social][9]


[6]: https://pixelfed.de/
[7]: https://pix.tedomum.net/
[8]: https://pix.diaspodon.fr/
[9]: https://pixelfed.social/earth

```

> Una vez que tengas un documento Markdown similar al de arriba (sin *header* ni *footer*) y ademas este completa la traducción puedes considerar un trabajo bien hecho! Gracias amigo :)