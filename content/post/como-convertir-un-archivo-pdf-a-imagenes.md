---
author: alex
categories:
- bash
- how to
- linux
color: '#2196F3'
date: '2016-01-01'
lastmod: 2017-03-15T18:26:24+01:00
description: "El otro día me hacía falta convertir cada una de las páginas  de un documento pdf a imágenes individuales, con un poco de búsqueda en google  lo solucioné y hoy lo comparto con vosotros."
mainclass: linux
url: /como-convertir-un-archivo-pdf-a-imagenes/
tags:
- como convertir pdf en imagen
- convertir pdf a jpg
- convertir pdf en imagenes
- imagemagick
- pdf a imagenes
- pdf to imagen
title: "Cómo convertir un archivo pdf a imágenes"
---

<figure>
    <amp-img sizes="(min-width: 128px) 128px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive" title="sh" src="/img/2012/07/sh1.png" alt="" width="128px" height="128px" />
</figure>

El otro día me hacía falta convertir cada una de las páginas de un documento pdf a imágenes individuales, con un poco de búsqueda en google lo solucioné y hoy lo comparto con vosotros.

Es necesario tener instalado el paquete imagemagick, si no lo tenemos instalado ejecutamos:

```bash
sudo aptitude install imagemagick
```

Tras instalarlo basta con ejecutar el comando siguiente:

```bash
convert foo.pdf foo.png
```

La extensión de la imagen podemos cambiarla a jpg por ejemplo.

Si las imágenes resultan con poca calidad, podemos ejecutar el siguiente comando:

```bash
convert -density 400 foo.pdf -resize 25% foo.png
```

Espero que os sea útil si alguna vez lo necesitáis.

&nbsp;

Vía | <a href="http://www.cyberciti.biz/faq/howto-convert-a-pdf-file-to-an-image/" target="_blank">cyberciti</a> | <a href="http://www.imagemagick.org/discourse-server/viewtopic.php?f=10&t=13371" target="_blank">imagemagick.org</a>
