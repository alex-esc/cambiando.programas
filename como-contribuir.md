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

## ¿Como transformar una pagina de HTML a Markdown?

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
